---
layout: post
title:  "Command Check Sheet"
categories: Computer Science
---
* TOC
{:toc}

### [Eclispe Memory Analyzer (MAT)][mat-doc]

[mat-doc]: http://help.eclipse.org/index.jsp?topic=/org.eclipse.mat.ui.help/welcome.html

### [gdb][gdb]

[gdb]: https://sourceware.org/gdb/current/onlinedocs/gdb/
1. [GDB: Debug native part of java application (C/C++ libraries and JDK)][gdb-java]
1. [GDB Internals from The Architecture of Open Source Applications][gdb-internals]
1. [ptrace][ptrace]

Some interesting commands:

```sh
gdb --batch --pid 51689 -ex "dump memory test.dum 0x7ff874000000  0x7ff87400ffff"

```

[gdb-java]: https://medium.com/@pirogov.alexey/gdb-debug-native-part-of-java-application-c-c-libraries-and-jdk-6593af3b4f3f
[gdb-internals]: https://www.aosabook.org/en/gdb.html 
[ptrace]: https://man7.org/linux/man-pages/man2/ptrace.2.html

### [java][java]

1. [What is Java Batch Mode: -Xbatch?][-xbatch]
1. [Eclipse OpenJ9™ virtual machine (VM)][openj9] 
1. [When to use -Xbootclasspath on HotSpot?][-Xbootclasspath]
1. [Java Native Access (JNA) vs JNI][jna]
1. [Understanding Java 9 Modules][module]
1. [ASM is an all purpose Java bytecode manipulation and analysis framework][asm]
1. [Java vs. Native Agents – And How It Affects Your Code][agents]
1. [Collecting and reading G1 garbage collector logs][g1gc]
1. [What is Unlock Diagnostic VM Options: -XX:+UnlockDiagnosticVMOptions?][unlock]
1. [JVM Anatomy Quark #12: Native Memory Tracking][shipilev-nmt]
1. [It's all about buffers: zero-copy, mmap and Java NIO][direct-memory]



[java]: https://docs.oracle.com/en/java/javase/19/docs/specs/man/java.html
[-xbatch]: https://answers.ycrash.io/question/-what-is-java-batch-mode--xbatch?q=649
[openj9]: https://www.eclipse.org/openj9/
[-Xbootclasspath]: http://xmlandmore.blogspot.com/2012/09/when-to-use-xbootclasspath-on-hotspot.html
[jna]: https://github.com/java-native-access/jna
[module]: https://www.oracle.com/corporate/features/understanding-java-9-modules.html
[asm]: https://asm.ow2.io/
[agents]: https://www.overops.com/blog/double-agent-java-vs-native-agents
[g1gc]: https://www.redhat.com/en/blog/collecting-and-reading-g1-garbage-collector-logs-part-2
[unlock]: https://answers.ycrash.io/question/what-is-unlock-diagnostic-vm-options--xxunlockdiagnosticvmoptions?q=701
[shipilev-nmt]: https://shipilev.net/jvm/anatomy-quarks/12-native-memory-tracking/
[direct-memory]: https://xunnanxu.github.io/2016/09/10/It-s-all-about-buffers-zero-copy-mmap-and-Java-NIO/ 

