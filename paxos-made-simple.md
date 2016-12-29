# Paxos Made Simple

Leslie Lamport

01 Nov 2001

(this is a markdown version of [orignal](http://research.microsoft.com/en-us/um/people/lamport/pubs/paxos-simple.pdf))

## Abstract

The Paxos algorithm, when presented in plain English, is very simple.

## Content

1. [Introduction](#1-introduction)
2. [Introduction](#2-the-consensus-algorithm)
2.1. [Introduction](#21-the-problem)

## 1 Introduction

The Paxos algorithm for implementing a fault-tolerant distributed system
has been regarded as difficult to understand, perhaps because the original
presentation was Greek to many readers [5]. In fact, it is among the simplest
and most obvious of distributed algorithms. At its heart is a consensus
algorithm—the "synod" algorithm of [5]. The next section shows that this
consensus algorithm follows almost unavoidably from the properties we want
it to satisfy. The last section explains the complete Paxos algorithm, which
is obtained by the straightforward application of consensus to the state machine
approach for building a distributed system—an approach that should
be well-known, since it is the subject of what is probably the most often-cited
article on the theory of distributed systems [4].

## 2 The Consensus Algorithm

### 2.1 The Problem

Assume a collection of processes that can propose values. A consensus algorithm
ensures that a single one among the proposed values is chosen. If
no value is proposed, then no value should be chosen. If a value has been
chosen, then processes should be able to learn the chosen value. The safety
requirements for consensus are:

+ Only a value that has been proposed may be chosen,
+ Only a single value is chosen, and
+ A process never learns that a value has been chosen unless it actually
has been.

We won’t try to specify precise liveness requirements. However, the goal is
to ensure that some proposed value is eventually chosen and, if a value has
been chosen, then a process can eventually learn the value.

We let the three roles in the consensus algorithm be performed by three
classes of agents: __proposers__, __acceptors__, and __learners__. 
In an implementation,
a single process may act as more than one agent, but the mapping from
agents to processes does not concern us here.

Assume that agents can communicate with one another by sending messages.
We use the customary asynchronous, non-Byzantine model, in which:

+ Agents operate at arbitrary speed, may fail by stopping, and may
restart. Since all agents may fail after a value is chosen and then
restart, a solution is impossible unless some information can be remembered
by an agent that has failed and restarted.
+ Messages can take arbitrarily long to be delivered, can be duplicated,
and can be lost, but they are not corrupted.

### 2.2 Choosing a Value

The easiest way to choose a value is to have a single acceptor agent. A proposer
sends a proposal to the acceptor, who chooses the first proposed value
that it receives. Although simple, this solution is unsatisfactory because the
failure of the acceptor makes any further progress impossible.

So, let’s try another way of choosing a value. Instead of a single acceptor,
let’s use multiple acceptor agents. A proposer sends a proposed value to a
set of acceptors. An acceptor may __accept__ the proposed value. The value is
chosen when a large enough set of acceptors have accepted it. How large is
large enough? To ensure that only a single value is chosen, we can let a large
enough set consist of any majority of the agents. Because any two majorities
have at least one acceptor in common, this works if an acceptor can accept
at most one value. (There is an obvious generalization of a majority that
has been observed in numerous papers, apparently starting with [3].)

In the absence of failure or message loss, we want a value to be chosen
even if only one value is proposed by a single proposer. This suggests the
requirement:

    P1. An acceptor must accept the first proposal that it receives.

But this requirement raises a problem. Several values could be proposed by
different proposers at about the same time, leading to a situation in which
every acceptor has accepted a value, but no single value is accepted by a
majority of them. Even with just two proposed values, if each is accepted by
about half the acceptors, failure of a single acceptor could make it impossible
to learn which of the values was chosen.
