---
layout: post
title:  "curiosity"
categories: curiosity 
---

* TOC
{:toc}


# Curiosity

“The important thing is not to stop questioning. Curiosity has its own reason for existence. One cannot help but be in awe when he contemplates the mysteries of eternity, of life, of the marvelous structure of reality. It is enough if one tries merely to comprehend a little of this mystery each day.
—"Old Man's Advice to Youth: 'Never Lose a Holy Curiosity.'" LIFE Magazine (2 May 1955) p. 64”

## How to

### How to transactional?

1. transaction -> ACID
      1. Atomic, -> switch reference.
      1. Consistency -> coordination.
         1. concurrency
         1. consistency model
      1. Isolated, -> virtualization.
      1. durable -> replica

1. [chain replication](https://www.cs.cornell.edu/home/rvr/papers/OSDI04.pdf)

### How to export DDB data to s3?

Daily scan the whole DDB table is very ineffcient and expensive. Obsolete ways:

1. https://github.com/audienceproject/spark-dynamodb
1. https://github.com/awslabs/emr-dynamodb-connector

Publish delta and do some compactions sounds promising.

PITR sounds promising:

1. https://aws.amazon.com/blogs/aws/new-export-amazon-dynamodb-table-data-to-data-lake-amazon-s3/
1. https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/S3DataExport.HowItWorks.html

Glue offers an out of box way to export ddb to s3 regularly.

1. https://aws.amazon.com/blogs/big-data/accelerate-amazon-dynamodb-data-access-in-aws-glue-jobs-using-the-new-aws-glue-dynamodb-elt-connector/

Idea: Write a CDK Construct which setup a pipeline to export DDB to s3 regularly.

### How to increase read throughput for remote encrypted files?

How to increase read throughput for remote encrypted files? For example, to read
S3 files encrypted in AES.

Check [code repo][code] for implementation.

Will [java virtual threads][java-virtual-threads] help?

How to record context switch?

[code]: https://github.com/wangzhihao/read-performance
[java-virtual-threads]: https://www.infoq.com/articles/java-virtual-threads/

## Others

1. The Elements of Statistical Learning by Jerome H. Friedman, Robert Tibshirani, and Trevor Hastie
2. [MultipleVariable Calculus](https://ocw.mit.edu/courses/mathematics/18-02sc-multivariable-calculus-fall-2010/syllabus/)
    1. [Determinant history](https://www.youtube.com/watch?v=Vg1e2FEpf9w)




1. **vision prosthesis**. to bring sight back to blindness. 
    1. Current machine-human interface is still limited to metals/wires alike (e.g. [Argus II](https://en.wikipedia.org/wiki/Argus_retinal_prosthesis)), which causes inflammation or rejection. To change that, a new material is desirable, which should be benefit from nano-technology and biology oriented.
2. **nano-technology**. It’s helpful to understand nano-technology by study the current cellular components and how they works. For example, a ribosome.
3. **ribosome.** How a ribosome works? How does the ribosome know to produce the protein? Who drive the actions? By which “force”?
    1. To answer such questions. We enter the domain of **Molecular Biology**, which tells us the process of transcription and translate of DNA and RNA. To understand the “force” part, We need to study **bio-chemistry.**
    2. Links
        1. https://www.quora.com/What-are-some-good-books-on-molecular-biology
        2. https://aklectures.com/
        3. https://www.nature.com/scitable/topicpage/ribosomes-transcription-and-translation-14120660
        4. https://www.quantamagazine.org/
4. Is life just a bunch of chemistry reactions?
    1. Links
        1. https://gmwgroup.harvard.edu/chemical-origins-life
5. What is consciousness? Does animal have it?
    1. Links
        1. https://en.wikipedia.org/wiki/Animal_consciousness
6. How to explain chemistry bond?
    1. Quantum mechanics?
7. What is Quantum mechanics?
    1. Does God Play Dice with the Universe?
    2. Links
        1. https://www.youtube.com/watch?v=msrl597rKKM
        2. https://en.wikipedia.org/wiki/Quantum_nonlocality
        3. https://www.nature.com/articles/35000514
        4. https://www.pnas.org/content/111/31/11281
        5. https://www.quora.com/Is-non-locality-of-quantum-entanglement-proved-beyond-any-doubts
        6. https://en.wikipedia.org/wiki/Bell%27s_theorem
        7. https://en.wikipedia.org/wiki/Bell_test
        8. https://www.youtube.com/watch?v=z1twSZF4fLM
        9. https://www.nature.com/articles/nature15759
        10. https://book.douban.com/subject/1467022/
8. Open problems
    1. Links
        1. https://en.wikipedia.org/wiki/Lists_of_unsolved_problems
        2. [Problems in Computer vision](https://www.youtube.com/watch?v=tOiwKqyocI8)
        3. scene understanding
        4. CVPR
        5. [Frame_problem](https://en.wikipedia.org/wiki/Frame_problem) [【1】](https://medium.com/@jockeyng/%E6%A1%86%E6%9E%B6%E5%95%8F%E9%A1%8C-1686bda35d7b)
9. How can I use computer to help in a practical way?
10. How to avoid cold start issue (to publish stale data to downstreams when replay in streaming processing like kafka/flink?)
    1. How to reuse the same destination when update flink sql?
    2. Invalid Problem: How to add backfill functionality to flink? [Replay is preferred]
        1. Easy: visibility to kafka. (kafka to DDB? / spark scan)
        2. backfill vs replay. Backfill is to send more inflow events, while replay keeps inflow events unchanged but just re-consume them. Flink/kafka follows replay pattern instead of backfill pattern. Sometimes the CDCNormalizer will make backfill ineffective.
            1. Contract: As long as the kafka is right. It’s consumers’ responsibility to replay. If the kafka is wrong, It’s provider’s responsibility to fix.
    3. A basic blue-green deployment is already good enough. [rollback also supported]. The only problem is some cold start issue. But we can argue if it really matters.
        1. Need a way to quantify the staleness, so that to quantify the severeness of cold start issue.
            1. We used to have an end-to-end metrics which takes two timestamps, one at the entry point of datapath, another at the sink point of elasticsearch. The difference between them is the latency. However, such a way can’t measure correctly the staleness of replay.
            2. The above way is bad when checkpoint happens.
            3. To improve the checkpoint issue. We can make the update by checkpoint invalid, by checking if the value it’s the same, we only make the first occurrence valid ([code](https://code.amazon.com/packages/ICatFlinkUDF/blobs/mainline/--/src/main/java/com/amazon/icat/udf/LatencyUDF.java)). Similar to a deduper. 

### Curiosity in Daily Work

1. **Flink application evolvement.**
2. **Flink visibility.**
3. **Flink join priotization.** In `a join b join c ` can I prioritize *c* while allow *a* and *b* to delay more. 
    1. Restock Team wants the recommendation updates reflect immediately whereas other attributes like price can be delayed a bit more.
    2. One option is to remove the traffic control at the output level (i.e. the 1min window implemented by guangheng), but apply the traffic control at input level. Leave the recommendation input unconstraint.
4. **An easy and better way to monitor & quantify flink data delay.**
5. **Can we exempt all unknowns?** NA is about 1.6M.







