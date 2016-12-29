[Blog](//blog.gobyoung.com/) / [Books](//blog.gobyoung.com/books) /

# Readings in Distributed Systems

## Systems
Graduate level operating systems courses don't typically have notes - they all come with long reading lists taken from SOSP and other places. In this way, systems research is a bit more like a humanities subject: it's vital to read the primary sources.

+ [Cornell CS 614 - Advanced Course in Computer Systems](http://www.cs.cornell.edu/Courses/cs614/2007fa/) - Ken Birman teaches this course. The readings cover more distributed systems research than is typical (which I am in favour of!). In fact, there's barely anything on traditional internal OS topics like filesystems or memory management. There's some worthwhile commentary at the bottom of the page.
+ [Princeton COS 518 - Advanced Operating Systems](https://www.cs.princeton.edu/courses/archive/fall13/cos518/) - short and snappy reading list of two papers per topic, covering some interesting stuff like buffering inside the operating system, and L4.
+ [Stanford CS240 - Advanced Topics in Operating Systems](http://www.stanford.edu/class/cs240/) - an interesting and concise set of readings. A presentation on Firefox internals is a course-specific highlight.
+ [Harvard CS264 - Peer-to-Peer Systems](http://www.eecs.harvard.edu/~mema/courses/cs264/cs264.html) - No notes but a useful collection of papers surveying from CAN and Chord to Skype.
+ [CSE 552 - Distributed Systems](https://courses.cs.washington.edu/courses/cse552/13au/) - University of Washington graduate distributed systems course. Thoughtfully selected readings.
+ [CMU 15-712 - Advanced and Distributed Operating Systems](http://www.cs.cmu.edu/~15712/)
+ [UIUC CS 525 - Advanced Distributed Systems](https://courses.engr.illinois.edu/cs525/sp2016/) - long list of readings, drawn mostly from the last ten years or so, focusing on applications.
+ [Cornell CS6452 - Datacenter Networks and Services](http://www.cs.cornell.edu/courses/cs6452/2012sp/lectures.php) - networking focused - but by no means exclusively.
+ [MIT 6.824 - Distributed Systems](https://pdos.csail.mit.edu/6.824/) - A modern distributed systems with go, raft and other new things.

## Databases
+ [Brown CSCI 2270 - Advanced Topics in Database Management](http://www.cs.brown.edu/courses/cs227/papers.html) - no notes but a good set of [readings](http://www.cs.brown.edu/courses/cs227/papers.html). Does a good job of categorising the last ~15 years of distributed and parallel database research which has moved away from shared-something RDBMSs.

## Distributed Algorithms

+ [MIT 6.852 - Distributed Algorithms](http://courses.csail.mit.edu/6.852/08/) - Goodish lecture slides, detailed but manageable set of readings and some homework problems. Lectured by Professor Lynch at MIT, who literally wrote the book on the subject.
+ [Distributed Algorithms Lecture Notes](http://citeseer.ist.psu.edu/120246.html) - Very readable set of lecture notes on distributed algorithms, for a course given in 1993 at the Technion in Israel (I think).
+ [MIT 6.885 - Distributed Algorithms for Mobile Wireless Ad-Hoc Networks](http://citeseer.ist.psu.edu/120246.html) - One of the only courses on this particular niche subject. Taught simultaneously by Jennifer Welch and Nancy Lynch. Notes are very good, reading lists is very comprehensive and there are also some good handouts!

## Data Structures and Algorithms
+ [MIT 6.854J (OCW) - Advanced Algorithms](http://dspace.mit.edu/html/1721.1/36897/6-854JFall-1999/OcwWeb/Electrical-Engineering-and-Computer-Science/6-854JAdvanced-AlgorithmsFall1999/LectureNotes/index.htm) - A good first course after familiarity with Cormen et. al. is achieved. Topics include competitive queues, splay trees, six lectures on flow algorithms, linear programming and computational geometry. Lecturer's own notes are sparse, but the scribed notes are very useful.
+ [MIT 6.851 - Advanced Data Structures](http://courses.csail.mit.edu/6.851/spring07/lec.html) - supercedes the below course I think, both taught by the legendary Erik Demaine. Worth keeping the below one around as well, since the notes are slightly different as are the topics covered.
+ [MIT 6.897 - Advanced Data Structures](http://courses.csail.mit.edu/6.897/spring05/index.html) - good coverage of advanced topics including dynamic graphs, succinct data structures and data structures for integers. Scribe notes are excellent, lecturer's own hand-written notes less so.
+ [Chicago CS369E - Expanders in Computer Science](http://ttic.uchicago.edu/~prahladh/teaching/05spring/) - graduate level course on expander graphs and their applications to computer science. Notes are excellent.
+ [Harvard CS225 - Pseudorandomness](http://www.courses.fas.harvard.edu/~cs225/Lectures/) - good scribe notes, covers randomized algorithms, quite a lot on expander graphs etc.
+ [Yale 500A - Spectral Graph Theory and its Applications](http://www.cs.yale.edu/homes/spielman/eigs/) - slightly rambling but clear and interesting lecturer written notes.
+ [UIUC CS573: Algorithmic Game Theory](http://www.cs.uiuc.edu/homes/chekuri/teaching/spring2008/agt.htm) - good scribe notes and a pointer to a massive online text book.
+ [Cornell CS683 - Advanced Algorithms](http://www.cs.cornell.edu/Courses/cs683/2001SP/Default.htm) - detailed web page, notes and readings. Focus is on approximation algorithms, linear programming and randomisation.
+ [Wisconsin CS787 - Advanced Algorithms](http://pages.cs.wisc.edu/~shuchi/courses/787-F07/) - decent notes and readings. Linear programming, network flows, approximation and randomisation, plus some interesting stuff on online algorithms.
+ [UIUC CS 373 - Combinatorial Algorithms](http://compgeom.cs.uiuc.edu/~jeffe/teaching/373/) - a senior undergraduate course in mainly advanced topics from CLRS with outstanding notes.

## Discrete Mathematics and Probability
+ [MIT 6.042J (OCW)](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-042j-mathematics-for-computer-science-fall-2010/) - Elementary discrete maths, including graph theory and some combinatorics. Lecture slides are available, and good, but the real meat is in the readings.

# Awesome Distributed Systems

Copied from [theanalyst/awesome-distributed-systems](https://github.com/theanalyst/awesome-distributed-systems)

A (hopefully) curated list on awesome material on distributed systems, inspired by
other awesome frameworks like [awesome-python](https://github.com/vinta/awesome-python).
Most links will tend to be readings on architecture itself rather than code itself.

## Bootcamp
Read things here before you start.
- [CAP Theorem](http://en.wikipedia.org/wiki/CAP_theorem), Also [plain english](http://ksat.me/a-plain-english-introduction-to-cap-theorem/) explanation
- [Fallacies of Distributed Computing](http://en.wikipedia.org/wiki/Fallacies_of_distributed_computing), expect things to break, *everything*
- [Distributed systems theory for the distributed engineer](http://the-paper-trail.org/blog/distributed-systems-theory-for-the-distributed-systems-engineer/), most of the papers/books in the blog might reappear in this list again. Still a good BFS approach to distributed systems.
- [FLP Impossibility Result (paper)](http://cs-www.cs.yale.edu/homes/arvind/cs425/doc/fischer.pdf), an easier [blog post](http://the-paper-trail.org/blog/a-brief-tour-of-flp-impossibility/) to follow along
- [An Introduction to Distributed Systems](https://github.com/aphyr/distsys-class) @aphyr's excellent introduction to distributed systems 

## Books
- [Distributed Systems for fun and profit](http://book.mixu.net/distsys/single-page.html) [Free]
- [Distributed Systems Principles and Paradigms, Andrew Tanenbaum](http://www.amazon.com/Distributed-Systems-Principles-Paradigms-2nd/dp/0132392275) [Amazon Link]
- [Scalable Web Architecture and Distributed Systems](http://www.aosabook.org/en/distsys.html) [Free]
- [Principles of Distributed Systems](http://dcg.ethz.ch/lectures/podc_allstars/lecture/podc.pdf) [ETH Zurich University]
- [Making reliable distributed systems in the presence of software errors](http://www.erlang.org/download/armstrong_thesis_2003.pdf), Joe Amstrong's (Author of Erlang) PhD thesis 
- [Designing Data Intensive Applications](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321) [Amazon Link]

## Papers
Must read papers on distributed systems. While nearly *all* of Lamport's work should feature here, just adding a few that *must* be read.
- [Times, Clocks and Ordering of Events in Distributed Systems](http://research.microsoft.com/en-us/um/people/lamport/pubs/time-clocks.pdf) Lamport's paper, the Quintessential distributed systems primer

### Storage & Databases
- [Dynamo: Amazon's Highly Available Key Value Store](http://bnrg.eecs.berkeley.edu/~randy/Courses/CS294.F07/Dynamo.pdf)
- [Bigtable: A Distributed Storage System for Structured Data](http://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)
- [The Google File System](http://static.googleusercontent.com/external_content/untrusted_dlcp/research.google.com/en/us/archive/gfs-sosp2003.pdf)
- [Cassandra: A Decentralized Structured Storage System](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.161.6751&rep=rep1&type=pdf) Inspired heavily by Dynamo
- [CRUSH: Controlled, Scalable, Decentralized Placement of Replicated Data](http://www.ssrc.ucsc.edu/Papers/weil-sc06.pdf), the algorithm for the basis of Ceph distributed storage system, for the architecture itself read [RADOS](http://ceph.com/papers/weil-rados-pdsw07.pdf)

### Messaging systems
- [The Log: What every software engineer should know about real-time data's unifying abstraction](http://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying), a somewhat long read, but covers brilliantly on logs, which are at the heart of most distributed systems
- [Kafka: a Distributed Messaging System for Log Processing](http://notes.stephenholiday.com/Kafka.pdf)

### Distributed Consensus
- [The Part Time Parliament](http://research.microsoft.com/en-us/um/people/lamport/pubs/lamport-paxos.pdf) Paxos, Lamport's original Paxos paper, a bit difficult to understand, may require multiple passes
- [Paxos Made Simple](paxos-made-simple.html) - [Origin](http://research.microsoft.com/en-us/um/people/lamport/pubs/paxos-simple.pdf), a more terse readable Paxos paper by Lamport himself. Shorter and more easier compared to the original.
- [The Chubby Lock Service for loosely coupled distributed systems](http://static.googleusercontent.com/media/research.google.com/en//archive/chubby-osdi06.pdf) Google's lock service used for loosely coupled distributed systems. Sort of Paxos as a Service for building other distributed systems. Primary inspiration behind other Service Discovery & Coordination tools like Zookeeper, etcd, Consul etc.
- [Paxos made live - An engineering perspective](http://research.google.com/archive/paxos_made_live.html) Google's learning while implementing systems atop of Paxos. Demonstrates various practical issues encountered while implementing a theoritical concept.
- [Raft Consensus Algorithm](https://raftconsensus.github.io/) An alternative to Paxos for distributed consensus, that is much simpler to understand. Do checkout an [interesting visualization of raft](http://thesecretlivesofdata.com/raft/)

### Testing, monitoring and tracing
While designing distributed systems are hard enough, testing them is even harder. 
- [Dapper](http://static.googleusercontent.com/media/research.google.com/en//pubs/archive/36356.pdf), Google's large scale distributed-systems tracing infrastructure, this was also the basis for the design of open source projects such as [Zipkin](http://zipkin.io/), [Pinpoint](https://github.com/naver/pinpoint) and [HTrace](http://htrace.incubator.apache.org/).

## Courses
- [Cloud Computing Concepts](https://class.coursera.org/cloudcomputing-001), University of Illinois
- [CMU: Distributed Systems](http://www.cs.cmu.edu/~dga/15-440/F12/syllabus.html) in Go Programming Language
- [Software Defined Networking](https://www.coursera.org/course/sdn) , Georgia Tech.
- [ETH Zurich: Distributed Systems](http://dcg.ethz.ch/lectures/podc_allstars/)
- [ETH Zurich: Distributed Systems Part 2](http://dcg.ethz.ch/lectures/distsys), covers  Distributed control algorithms, communication models, fault-tolerance among other things. In particular fault tolerence issues (models, consensus, agreement) and replication issues (2PC,3PC, Paxos), which are critical in understanding distributed systems are explained in great detail.

## Blogs and other reading links
- [Notes on Distributed Systems for Young Bloods](http://www.somethingsimilar.com/2013/01/14/notes-on-distributed-systems-for-young-bloods/)
- [High Scalability](http://highscalability.com/) Several architectures of huge internet services, for eg [twitter](http://highscalability.com/blog/2013/7/8/the-architecture-twitter-uses-to-deal-with-150m-active-users.html), [whatsapp](http://highscalability.com/blog/2014/2/26/the-whatsapp-architecture-facebook-bought-for-19-billion.html)
- [There is No Now](http://queue.acm.org/detail.cfm?id=2745385), Problems with simultaneity in distributed systems
- [Turing Lecture: The Computer Science of Concurrency: The Early Years](http://cacm.acm.org/magazines/2015/6/187316-turing-lecture-the-computer-science-of-concurrency/fulltext), An article by Leslie Lamport on concurrency
- [The Paper Trail](http://the-paper-trail.org/blog/tag/distributed-systems/) blog, a very readable blog covering various aspects of distributed systems
- [aphyr](https://aphyr.com/tags/Distributed-Systems), Posts on [jepsen](https://github.com/aphyr/jepsen) series are pretty awesome
- [All Things Distributed](http://www.allthingsdistributed.com/) - Wernel Vogel's (Amazon CTO) blog on distributed systems 
- [Distributed Systems: Take Responsibility for Failover](http://ivolo.me/distributed-systems-take-responsibility-for-failover/)
- [The C10K problem](http://www.kegel.com/c10k.html)
- [On Designing and Deploying Internet-Scale Services](http://static.usenix.org/event/lisa07/tech/full_papers/hamilton/hamilton_html/)
- [Files are hard](http://danluu.com/file-consistency/) A blog post on filesystem consistency, pretty important to read if you are into distributed storage or databases.
- [Distributed Systems Testing: The Lost World](http://tagide.com/blog/research/distributed-systems-testing-the-lost-world/) Testing distributed systems are hard enough, a well researched blog post which again covers a lot of links to various approaches and other papers

## Meta Lists

Other lists like this one

- [Readings in distributed systems](http://christophermeiklejohn.com/distributed/systems/2013/07/12/readings-in-distributed-systems.html)
- [Distributed Systems meta list](https://gist.github.com/macintux/6227368)
- [List of required readings for Distributed Systems](http://www.andrew.cmu.edu/course/15-749/READINGS/required/) Part of CMU's Engineering Distributed Systems course
- [The Distributed Reader](http://reiddraper.github.io/distreader/)
- [A Distributed Systems Reading List](https://dancres.github.io/Pages/), A collection of material, mostly papers on Distributed Systems Theory as well as seminal industry papers 
- [Distributed Systems Readings](https://henryr.github.io/distributed-systems-readings/), A comprehensive list of online courses related to distributed systems 

