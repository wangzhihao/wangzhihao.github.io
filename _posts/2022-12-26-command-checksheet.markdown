---
layout: post
title:  "Command Check Sheet"
categories: Computer Science
---
* TOC
{:toc}

## One-liner

1. **bcc install**: on EC2, run `sudo yum install bcc` and you will find tools under
`/usr/share/bcc/tools/`.
1. **perf install**: on EC2, run `sudo yum install perf`.
1. **memory leak**: [bcc memleak][bcc-memleak] instruments all alloc functions which is great
to detect continous leaking.


[bcc-memleak]: https://github.com/iovisor/bcc/blob/master/tools/memleak_example.txt
