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
1. **ecs exec**
    ```
    aws ecs execute-command  \
        --region us-east-1 \
        --cluster EcsCluster-ProdNA-ClusterEB0386A7-xCOnJWJzmOR3 \
        --task 10bb93e288194bc1bd1ffd2a8d1663fe \
        --container web \
        --command "/bin/bash" \
        --interactive
    ```
1. **memory leak**: [bcc memleak][bcc-memleak] instruments all alloc functions which is great
to detect continous leaking.
1. **perf install**: on EC2, run `sudo yum install perf`.
1. **traceroute**, [geotraceroute](https://geotraceroute.com/), trace a request in network.
1. **vim**: 
    ```
    bemol --watch
    :CocStart
    :CocInstall coc-java
    :CocInstall coc-rust-analyzer
    ```





## Vim basic requirements
1. **DOC** `Shift + K`: to show the documentation. Then use `CTRL + f` or `CTRL + b` to page up and down.
1. **Format** To format line 3 to 29 `:3, v29G, \f`, to format the whole file `:Format`. Disable auto format on purpose.
1. **Organize Imports** `:OR`
1. **Goto Definition** `gd`
1. Pending: Auto import when typing. (type OR, avoid automatically rewrite)
1. Pending: tab to auto expand and select the first hint. (use cr to confirm)

[bcc-memleak]: https://github.com/iovisor/bcc/blob/master/tools/memleak_example.txt
