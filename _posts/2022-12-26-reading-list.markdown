---
layout: post
title:  "Reading List"
categories: Computer Science
---
* TOC
{:toc}


## Reading

1. [coc-nvim.txt](https://github.com/neoclide/coc.nvim/blob/master/doc/coc.txt)

## Important papers

### Distributed System

1. **PAXOS**: [Lamport, Leslie](https://en.wikipedia.org/wiki/Leslie_Lamport). "The part-time parliament." *Concurrency: the Works of Leslie Lamport*. [2019. 277-317](tel:2019277317). [[paper](https://lamport.azurewebsites.net/pubs/lamport-paxos.pdf), [impl](https://code.amazon.com/packages/LSD/blobs/mainline-2.0/--/src/lsd/paxos/PaxosLSD.java), 30% read]
2. **Zookeeper Atomic broadcast:** [Junqueira, Flavio P](https://scholar.google.com/citations?user=48qKfREAAAAJ&hl=en)., [Benjamin C. Reed](https://scholar.google.com/citations?user=LpByivcAAAAJ&hl=en&oi=sra), and Marco Serafini. "Zab: High-performance broadcast for primary-backup systems." *2011 IEEE/IFIP 41st International Conference on Dependable Systems & Networks (DSN)*. IEEE, 2011. [[paper](https://marcoserafini.github.io/papers/zab.pdf), ]
3. **Raft**: [Ongaro, Diego](https://ongardie.net/), and John Ousterhout. "In search of an understandable consensus algorithm." *2014 USENIX Annual Technical Conference (Usenix ATC 14)*. 2014.
4. **Chain Replication**: [Van Renesse, Robbert](https://www.cs.cornell.edu/home/rvr/), and Fred B. Schneider. "Chain Replication for Supporting High Throughput and Availability." *OSDI*. Vol. 4. No. 91–104. 2004. [[paper](http://www.cs.cornell.edu/home/rvr/papers/OSDI04.pdf), [impl](https://code.amazon.com/packages/AlfBus/trees/mainline), 30% read]
5. **Consistency models**. https://jepsen.io/consistency [[analysis](https://quip-amazon.com/ajlKAVvFZfc9/Consistency-Models)]
6. **Consensus number.** Herlihy, Maurice. "Wait-free synchronization." *ACM Transactions on Programming Languages and Systems (TOPLAS)* 13.1 (1991): 124-149. [[dijkstra prize](https://www.podc.org/dijkstra/2003-dijkstra/)]
7. **Java Memory Model:** Manson, Jeremy, William Pugh, and Sarita V. Adve. "The Java memory model." *ACM SIGPLAN Notices* 40.1 (2005): 378-391.
8. **Race detection:** Flanagan, Cormac, and Stephen N. Freund. "FastTrack: efficient and precise dynamic race detection." *ACM Sigplan Notices* 44.6 (2009): 121-133. [[paper](https://users.soe.ucsc.edu/~cormac/papers/pldi09.pdf), [go race detection](https://www.uber.com/blog/dynamic-data-race-detection-in-go-code/), [fbinfer](https://fbinfer.com/docs/checker-racerd), [another paper](https://theory.stanford.edu/~aiken/publications/papers/pldi06.pdf)]

### Data Structure

1. **Consistent hashing**: [Karger, David](http://people.csail.mit.edu/karger/), et al. "Consistent hashing and random trees: Distributed caching protocols for relieving hot spots on the world wide web." *Proceedings of the twenty-ninth annual ACM symposium on Theory of computing*. 1997. [[paper](https://www.cs.princeton.edu/courses/archive/fall09/cos518/papers/chash.pdf), impl, read once]
2. **Bloom filter:** [Bloom, Burton H](https://www.quora.com/Where-can-one-find-a-photo-and-biographical-details-for-Burton-Howard-Bloom-inventor-of-the-Bloom-filter). "Space/time trade-offs in hash coding with allowable errors." *Communications of the ACM* 13.7 (1970): 422-426. [[paper](https://cs.pwr.edu.pl/cichon/2021_22_a/BigData/Bloom.pdf), impl, 50% read]
3. **LSM**: [O’Neil, Patrick](https://en.wikipedia.org/wiki/Patrick_O'Neil), et al. "The log-structured merge-tree (LSM-tree)." *Acta Informatica* 33.4 (1996): 351-385.[[paper](https://www.cs.umb.edu/~poneil/lsmtree.pdf), [impl](https://github.com/google/leveldb), 70% read]
4. **B-Tree**: [Bayer, Rudolf](https://en.wikipedia.org/wiki/Rudolf_Bayer), and Edward McCreight. "Organization and maintenance of large ordered indexes." *Software pioneers*. Springer, Berlin, Heidelberg, 2002. 245-262. [[paper](https://infolab.usc.edu/csci585/Spring2010/den_ar/indexing.pdf), ]
5. **Skip list**: [Pugh, William](http://www.cs.umd.edu/~pugh/). "Skip lists: a probabilistic alternative to balanced trees." *Communications of the ACM* 33.6 (1990): 668-676. [[paper](https://15721.courses.cs.cmu.edu/spring2018/papers/08-oltpindexes1/pugh-skiplists-cacm1990.pdf), [impl](https://github.com/google/leveldb/blob/main/db/skiplist.h), 70% read]

### Database

1. **LRU-K**: [O'neil, Elizabeth J](https://en.wikipedia.org/wiki/Elizabeth_O%27Neil) (mother)., [Patrick E. O'neil](https://en.wikipedia.org/wiki/Patrick_O'Neil), and Gerhard Weikum. "The LRU-K page replacement algorithm for database disk buffering." Acm Sigmod Record 22.2 (1993): 297-306.
2. **MVCC**: [Reed, David Patrick](https://en.wikipedia.org/wiki/David_P._Reed). *Naming and synchronization in a decentralized computer system*. Diss. Massachusetts Institute of Technology, 1978. [[paper](http://publications.csail.mit.edu/lcs/pubs/pdf/MIT-LCS-TR-205.pdf), 20% read]
3. **CodeGen**: [Neumann, Thomas](https://db.in.tum.de/~neumann/). "Efficiently compiling efficient query plans for modern hardware." *Proceedings of the VLDB Endowment* 4.9 (2011): 539-550. [[paper](https://www.vldb.org/pvldb/vol4/p539-neumann.pdf)]
4. **OCC:** [Kung, Hsiang-Tsung](https://en.wikipedia.org/wiki/H._T._Kung), and John T. Robinson. "On optimistic methods for concurrency control." *ACM Transactions on Database Systems (TODS)* 6.2 (1981): 213-226.

### Language

1. **Hoare logic:** Hoare, Charles Antony Richard. "An axiomatic basis for computer programming." *Communications of the ACM* 12.10 (1969): 576-580. [[paper](http://sunnyday.mit.edu/16.355/Hoare-CACM-69.pdf), [presentation](http://umathur3.web.engr.illinois.edu/documents/slides/hoare.pdf)]
2. **Coq**: https://coq.inria.fr/ 
3. [Jung, Ralf.](https://scholar.google.com/citations?user=zddokfoAAAAJ&hl=en&oi=sra) "Understanding and Evolving the Rust Programming Language." (2020). ([pdf](https://research.ralfj.de/phd/thesis-screen.pdf))
4. [The Rustonomicon](https://doc.rust-lang.org/nomicon/#the-rustonomicon)
5. Rust RFCs (e.g. RFC for [nll borrow checker](https://rust-lang.github.io/rfcs/2094-nll.html))
6. **Async Programming (Kotlin Coroutines):** Elizarov, Roman, et al. "Kotlin coroutines: design and implementation." *Proceedings of the 2021 ACM SIGPLAN International Symposium on New Ideas, New Paradigms, and Reflections on Programming and Software*. 2021. ([video link](https://dl.acm.org/doi/10.1145/3486607.3486751))
7. **G1 GC**: Detlefs, David, et al. "Garbage-first garbage collection." *Proceedings of the 4th international symposium on Memory management*. 2004.

### Memory Management

1. **Slab**. Bonwick, Jeff. "The slab allocator: An object-caching kernel memory allocator." *USENIX summer*. Vol. 16. 1994.
2. https://www.memorymanagement.org/

### Network

1. **TLS:** [[spec](https://www.rfc-editor.org/rfc/pdfrfc/rfc8446.txt.pdf)]

### Virtualization

1. **virtio:** [Russell, Rusty](https://en.wikipedia.org/wiki/Rusty_Russell). "virtio: towards a de-facto standard for virtual I/O devices." *ACM SIGOPS Operating Systems Review* 42.5 (2008): 95-103. [[paper](https://ozlabs.org/~rusty/virtio-spec/virtio-paper.pdf), [video](https://www.youtube.com/watch?v=FY-iQnrrOgk)]
2. Intel Virtualisation: How VT-x, KVM and QEMU Work Together [[link](https://binarydebt.wordpress.com/2018/10/14/intel-virtualisation-how-vt-x-kvm-and-qemu-work-together/)]

### Streaming
1. [Rethinking Stream Processing and Streaming Databases](https://www.risingwave-labs.com/blog/Rethinking_stream_processing_and_streaming_databases/) -- from RisingWave by [Yingjun Wu](https://twitter.com/YingjunWu) [1 time read]

### Others

1. **SSD**: https://en.wikipedia.org/wiki/Solid-state_drive
2. **REST**: [Fielding, Roy Thomas](https://en.wikipedia.org/wiki/Roy_Fielding). *Architectural styles and the design of network-based software architectures*. University of California, Irvine, 2000.[[paper](https://www.ics.uci.edu/~fielding/pubs/dissertation/fielding_dissertation.pdf), ]
3. **LLVM**: [Lattner, Chris](https://en.wikipedia.org/wiki/Chris_Lattner), and Vikram Adve. "LLVM: A compilation framework for lifelong program analysis & transformation." *International Symposium on Code Generation and Optimization, 2004. CGO 2004.*. IEEE, 2004. [[paper](https://llvm.org/pubs/2003-09-30-LifelongOptimizationTR.pdf), ]

## Technical papers

1. **Kafka:** Kreps, Jay, Neha Narkhede, and Jun Rao. "Kafka: A distributed messaging system for log processing." *Proceedings of the NetDB*. Vol. 11. 2011. [[paper](http://notes.stephenholiday.com/Kafka.pdf), ]
2. **Presto/Trino**: Sethi, Raghav, et al. "Presto: SQL on everything." *2019 IEEE 35th International Conference on Data Engineering (ICDE)*. IEEE, 2019.
3. **Ray:** Moritz, Philipp, et al. "Ray: A distributed framework for emerging {AI} applications." *13th USENIX Symposium on Operating Systems Design and Implementation (OSDI 18)*. 2018.
4. **Flink:** Carbone, Paris, et al. "Apache flink: Stream and batch processing in a single engine." Bulletin of the IEEE Computer Society Technical Committee on Data Engineering 36.4 (2015). [Flink Improvement Proposals](https://cwiki.apache.org/confluence/display/FLINK/Flink+Improvement+Proposals)
5. **Spark:** Zaharia, Matei, et al. "Resilient distributed datasets: A {Fault-Tolerant} abstraction for {In-Memory} cluster computing." *9th USENIX Symposium on Networked Systems Design and Implementation (NSDI 12)*. 2012. [Spark project improvement proposals](https://spark.apache.org/improvement-proposals.html)
6. **Mosh:** Winstein, Keith, and Hari Balakrishnan. "Mosh: An interactive remote shell for mobile clients." *2012 USENIX Annual Technical Conference (USENIX ATC 12)*. 2012.
7. **ZooKeeper:** Hunt, Patrick, et al. "{ZooKeeper}: Wait-free Coordination for Internet-scale Systems." *2010 USENIX Annual Technical Conference (USENIX ATC 10)*. 2010.
8. **Chubby:** [Burrows, Mike](https://en.wikipedia.org/wiki/Michael_Burrows). "The Chubby lock service for loosely-coupled distributed systems." *Proceedings of the 7th symposium on Operating systems design and implementation*. 2006.
9. **MapReduce:** Dean, Jeffrey, and Sanjay Ghemawat. "MapReduce: simplified data processing on large clusters." *Communications of the ACM* 51.1 (2008): 107-113.
10. **GFS**: [Ghemawat, Sanjay](https://en.wikipedia.org/wiki/Sanjay_Ghemawat), Howard Gobioff, and Shun-Tak Leung. "The Google file system." *Proceedings of the nineteenth ACM symposium on Operating systems principles*. 2003.
11. **Firecracker:** Agache, Alexandru, et al. "Firecracker: Lightweight virtualization for serverless applications." *17th USENIX symposium on networked systems design and implementation (NSDI 20)*. 2020. [[paper](https://www.usenix.org/system/files/nsdi20-paper-agache.pdf)]

## Important Code

**Tiny**

1. Kotlin Coroutines ([interface](https://github.com/JetBrains/kotlin/tree/master/libraries/stdlib/src/kotlin/coroutines), [jvm impl](https://github.com/JetBrains/kotlin/tree/master/libraries/stdlib/jvm/src/kotlin/coroutines) LoC < 1K, [scheduling](https://github.com/Kotlin/kotlinx.coroutines/blob/master/kotlinx-coroutines-core/jvm/src/scheduling/CoroutineScheduler.kt) LoC < 1K)
2. [DataTurboEMR](https://code.amazon.com/packages/DataTurboEMR/trees/heads/inv-health-mainline) (LoC: 2K)
3. [GoAmzn-LambdaGirp](https://code.amazon.com/packages/GoAmzn-LambdaGirp/trees/mainline) (LoC: 5K)

**Small**

1. [leveldb](https://github.com/google/leveldb) by [Jeffrey Dean](https://research.google/people/jeff/) et al. (LoC: 22K)
2. [java concurrent](https://github.com/openjdk/jdk/tree/master/src/java.base/share/classes/java/util/concurrent) (LoC: 29K)
3. [hotspot memory](https://github.com/openjdk/jdk/tree/master/src/hotspot/share/memory) (LoC: 12K, [wiki](https://wiki.openjdk.org/display/HotSpot))
4. [firecracker v 0.1.0](https://github.com/firecracker-microvm/firecracker/tree/v0.1.0) (LoC: 42K)
5. [coc.nvim](https://github.com/neoclide/coc.nvim) (LoC: 97K)

**Large**

1. [java](https://github.com/openjdk/jdk) [[code analysis](https://quip-amazon.com/JJbDA2Z6Fz6v/java-code-analysis)] (LoC: 16M)
2. [kafka](https://github.com/apache/kafka) by [Kreps, Jay](https://twitter.com/jaykreps?lang=en) et al. [[Code Analysis](https://quip-amazon.com/IUQOAlCppcA4/Kafka-Code-Analysis)] (LoC: 734K)
3. [zookeeper](https://github.com/apache/zookeeper) [[Code Analysis](https://quip-amazon.com/Gx4aATuBiGb5/Zookeeper-Analysis)] (LoC: 180K)

**Interest Pool**
[SkySailJavaAgent](https://code.amazon.com/packages/SkySailJavaAgent/trees/mainline)  (LoC: 12K) / [QLDB](https://code.amazon.com/packages/QLDB/trees/mainline) / 

## Course

1. Stanford, Introduction to logic by [Michael Genesereth](http://logic.stanford.edu/people/genesereth/genesereth.html) [[video](https://www.youtube.com/watch?v=AlR6_A8RHak), [site](http://intrologic.stanford.edu/homepage/index.html)]
2. UC Berkeley's *CS 162*: Operating Systems and Systems Programming. by [John Kubiatowicz](https://people.eecs.berkeley.edu/~kubitron/) [[link](https://www.youtube.com/playlist?list=PLMcZASLnrVs5qyBC-dc4bFRtC8ROPYmS0)]
3. [MIT 6.033 Computer System Engineering](https://dspace.mit.edu/bitstream/handle/1721.1/118791/6-033-spring-2009/contents/index.htm) by Robert Morris, Samuel Madden
4. [MIT 6.824: Distributed Systems](http://nil.csail.mit.edu/6.824/2020/schedule.html) by [Robert Morris](http://pdos.csail.mit.edu/~rtm/)
5. MIT 6.851 [ADVANCED DATA STRUCTURES](https://ocw.mit.edu/courses/6-851-advanced-data-structures-spring-2012/) by  [Prof. Erik Demaine](https://ocw.mit.edu/search?q=Prof.+Erik+Demaine)
6. MIT 6.858 [COMPUTER SYSTEMS SECURITY](https://ocw.mit.edu/courses/6-858-computer-systems-security-fall-2014/) by  [Prof. Nickolai Zeldovich](https://ocw.mit.edu/search?q=Prof.+Nickolai+Zeldovich)
7. MIT 8.962 [GENERAL RELATIVITY](https://ocw.mit.edu/courses/8-962-general-relativity-spring-2020/)
8. MIT 15.S12 BLOCKCHAIN AND MONEY
9. RUST Learning resources[from Amazon wiki](https://w.amazon.com/bin/view/RustLang#HLearningRust)
10. [CMU 15-721 Advanced Database Systems](https://15721.courses.cs.cmu.edu/spring2020/)
11. [CS 6120: Advanced Compilers: The Self-Guided Online Course](https://www.cs.cornell.edu/courses/cs6120/2022sp/self-guided/)
12. [CS144, Introduction to Computer Networking](https://www.youtube.com/watch?v=qAFI-2I7wPE&list=PLoCMsyE1cvdWKsLVyf6cPwCLDIZnOj0NS)
13. MIT 6.875 Foundations of Cryptography [[link](https://mit6875.github.io/fall2021.html)]

## Books

1. Herlihy, Maurice, et al. *The art of multiprocessor programming*. Newnes, 2020. [[pdf](https://cs.ipm.ac.ir/asoc2016/Resources/Theartofmulticore.pdf)]
2. Harper, Robert. *Practical foundations for programming languages*. Cambridge University Press, 2016.
3. Gregg, Brendan. *Systems performance: enterprise and the cloud*. Pearson Education, 2014. [[link](https://github.com/gg-daddy/ebooks/blob/master/Systems.Performance.Enterprise.and.the.Cloud.2013.10.pdf), [website](https://www.brendangregg.com/linuxperf.html)]
4. Warren, Henry S. *Hacker's delight*. Pearson Education, 2013.
5. Abelson, Harold, and Gerald Jay Sussman. *Structure and interpretation of computer programs*. The MIT Press, 1996.
6. Knuth, Donald Ervin. *The art of computer programming*. Pearson Education, 1997. [[v1](http://broiler.astrometry.net/~kilian/The_Art_of_Computer_Programming%20-%20Vol%201.pdf), [v2](https://doc.lagout.org/science/0_Computer%20Science/2_Algorithms/The%20Art%20of%20Computer%20Programming%20%28vol.%202_%20Seminumerical%20Algorithms%29%20%283rd%20ed.%29%20%5BKnuth%201997-11-14%5D.pdf), [v3](https://doc.lagout.org/science/0_Computer%20Science/2_Algorithms/The%20Art%20of%20Computer%20Programming%20%28vol.%203_%20Sorting%20and%20Searching%29%20%282nd%20ed.%29%20%5BKnuth%201998-05-04%5D.pdf), v4]
7. Hofstadter, Douglas R. *Gödel, escher, bach*. New York: Basic books, 1979.

## Specification

1. [SYSTEM V APPLICATION BINARY INTERFACE](http://www.sco.com/developers/devspecs/gabi41.pdf)
1. [RFC793: TRANSMISSION CONTROL PROTOCOL][rfc793] edited by [Jon Postel][Jon_Postel], invented by [Vint Cerf][Vint_Cerf] and [Bob Kahn][Bob_Kahn]. [1 time read].

[Jon_Postel]: https://en.wikipedia.org/wiki/Jon_Postel
[Vint_Cerf]: https://en.wikipedia.org/wiki/Vint_Cerf
[Bob_Kahn]: https://en.wikipedia.org/wiki/Bob_Kahn
[rfc793]: https://www.rfc-editor.org/rfc/pdfrfc/rfc793.txt.pdf


## Awards

1. [Turing Award](https://amturing.acm.org/byyear.cfm)
2. [Dijkstra Prize](https://www.podc.org/dijkstra)
3. [Programming Languages Achievement Award](https://www.sigplan.org/Awards/Achievement/)

## Questions

1. How to develop read-intensive and write intensive databases? What’s the difference?
2. How S3 handle hot spot?

## JVM

1. https://shipilev.net/jvm/anatomy-quarks/
2. https://a10y.github.io/post/2018-02-13-card-tables/
3. http://psy-lob-saw.blogspot.com/2014/10/the-jvm-write-barrier-card-marking.html

## Followings

1. Nitsan Wakart 
    1. [JCTools talk in InfoQ/QCONF](https://www.infoq.com/presentations/jctools-algorithms-optimization/)
    2. [Lock Free queue index](http://psy-lob-saw.blogspot.com/p/lock-free-queues.html)
2. Martin Thompson
    1. YOW! 2012 Martin Thompson ([blog](https://mechanical-sympathy.blogspot.com/), [linkedin](https://www.linkedin.com/in/martinjthompson/?originalSubdomain=uk)) - Lock-free Algorithms for Ultimate Performance ([video](https://www.youtube.com/watch?v=_uUkApe_yIk), [presentation](https://qconsf.com/sf2012/dl/qcon-sanfran-2012/slides/MartinThompson_LockFreeAlgorithmsForUltimatePerformanceMOVEDTOBALLROOMA.pdf))
3. Chris Newland ([linkedin](https://www.linkedin.com/in/chriswhocodes))
    1. https://blogs.oracle.com/javamagazine/post/java-hotspot-hsdis-disassembler
    2. https://www.infoq.com/presentations/jitwatch/


## Other candidates

1. https://go.dev/doc/effective_go
2. Most data structures like b-tree, kd-tree, r-tree , crc32, etc.
3. [Java Memory Model](https://rsim.cs.uiuc.edu/Pubs/popl05.pdf)
4. locks, concurrency, cache, page, 
5. https://dbdb.io/db/leveldb
6. https://www.vldb.org/pvldb/vol11/p2209-kersten.pdf
7. https://w.amazon.com/bin/view/AWS/CPR/
8. SSDs: https://w.amazon.com/bin/view/S3Team/DocumentGarden#SSDs
9. https://jepsen.io/consistency
10. https://www.cl.cam.ac.uk/~ey204/teaching/ACS/R244_2018_2019/papers/Kraska_SIGMOD_2018.pdf
11. https://w.amazon.com/bin/view/BigBird/
12. https://w.amazon.com/bin/view/BigBird/Development/StorageNode/NewHire/#HStorageNodearchitecture
13. https://w.amazon.com/bin/view/BigBird/Development/StorageNode
14. https://www.brendangregg.com/linuxperf.html
15. Meltdown & Spectre
16. https://broadcast.amazon.com/videos/571271  / https://w.amazon.com/bin/view/ELB/Teams/Falcon
17. https://www.cs.uoregon.edu/research/summerschool/summer13/curriculum.html
18. More MIT courses: https://ocw.mit.edu/search/?f=Lecture%20Videos&t=Computer%20Science
19. mmap
20. http://www.catb.org/esr/structure-packing/
    1. https://en.wikipedia.org/wiki/Data_structure_alignment
21. https://eli.thegreenplace.net/2018/measuring-context-switching-and-memory-overheads-for-linux-threads/




## Amateur 

### Music

1. Structural Hearing: Tonal Coherence in Music
2. On Piano Playing: Motion, Sound, and Expression

### Novel

1. The Little Prince
2. Kite Runner
3. The Old man and the sea
4. 生命不能承受之轻


### Cognitive Science
1. [Max Kleiman-Weiner](http://www.mit.edu/~maxkw/), Harvard
1. [Tobias Gerstenberg](https://cicl.stanford.edu/member/tobias_gerstenberg/)
1. [Computational Cognitive Science Lab](https://cocosci.princeton.edu/)
1. [Tom Griffiths](https://cocosci.princeton.edu/tom/tom.php)
1. Friedenberg, Jay, Gordon Silverman, and Michael J. Spivey. Cognitive science: an introduction to the study of mind. Sage Publications, 2021.
1. [Cognitive Science Society](https://cogsci.mindmodeling.org/)
1. [Stanford Cognitive Science Concentration: Approved Courses](https://symsys.stanford.edu/undergraduatesconcentrationscognitive-science-cogsci/cognitive-science-concentration-approved)


## Philosophy 
1. Perry, John. A dialogue on personal identity and immortality. Hackett Publishing, 1978.

### Others
1. Brain Computer Interface
    1. https://www.bci-award.com/Home
    1. https://synchron.com/
    1. https://en.wikipedia.org/wiki/Annual_BCI_Research_Award
1. Computer Music: https://ccrma.stanford.edu/
    1. Course: https://www.coursera.org/learn/audio-signal-processing/home/welcome
    2. Course: https://online.stanford.edu/courses/sohs-music0002-physics-based-sound-synthesis-games-and-interactive-systems
    3. https://ccrma.stanford.edu/academics/courses/course-history
    4. http://www.computermusic.org/
    5. Dannenberg, Roger B. "An on-line algorithm for real-time accompaniment." ICMC. Vol. 84. 1984.
    6. https://quod.lib.umich.edu/i/icmc/bbp2372.2018?rgn=full+text
1. https://en.wikipedia.org/wiki/Domain-driven_design
1. Suburban Nation: The Rise of Sprawl and the Decline of the American Dream
1. The restoration of the self 
1. [庄子](https://www.amazon.com/%E4%B8%AD%E5%8D%8E%E7%BB%8F%E5%85%B8%E5%90%8D%E8%91%97%E5%85%A8%E6%9C%AC%E5%85%A8%E6%B3%A8%E5%85%A8%E8%AF%91-%E5%BA%84%E5%AD%90-%E6%96%B9%E5%8B%87/dp/7101109527)
1. Nonviolent Communication

