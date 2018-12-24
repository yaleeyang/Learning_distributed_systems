# Learning distributed systems checkin history

Day 1: 2018/12/20 . 
Day 2: 2018/12/21

Youtube: [Distributed Systems in One Lesson by Tim Berglund](https://www.youtube.com/watch?v=Y6Ev8GIlbxc)

**Notes:**

- What is a distributed system?
  - A collection of independent computers that appear to its users as one computer. (Andrew Tannenbaum)
  - Three Characteristics:
    - The computers operate concurrently
    - The computers fail independently
    - The computers do not share a global clock
  - Distributed Storage
    - Single-master storage
    - Read replication
    - Sharding
    - Consistent hashing
    - Replication
    - Consistency: R + W > N
    - CAP theorem
  - Distributed Computation
    - MapReduce: Map, Shuffle, Reduce
    - Hadoop: MapReduce, Job management, HDFS
    - Spark: Scatter/gather, RDDs & DataSets, transform/action, Storage agnostic
    - Kafka: Real-time analysis, Streams only, No cluster required
    - Lambda architecture
  - Messaging
    - loosely coupling subsystems
    - consumed by subscribers
    - created by one or more producers
    - Organized into topics
    - Processed by brokers
    
Day 3: 2018/12/24 .
    
V.Buterin [Zk-SNARKs: Under the Hood](https://medium.com/@VitalikButerin/zk-snarks-under-the-hood-b33151a013f6) prerequisite step 1: [Quadratic Arithmetic Programs: from Zero to Hero](https://medium.com/@VitalikButerin/quadratic-arithmetic-programs-from-zero-to-hero-f6d558cea649)
    
**Notes:**

- zk-SNARKs cannot be applied to any computational problem directly; you have to convert the problem into the right “form” for the problem to operate on. The form is called a “quadratic arithmetic program” (QAP)
- 1. Flattening: we convert the original code, which may contain arbitrarily complex statements and expressions, into a sequence of statements that are of two forms:
  - x = y (where y can be a variable or a number)
  - x = y (op) z (where op can be +, -, *, / and y and z can be variables, numbers or themselves sub-expressions)
- 2. Gates to R1CS (rank-1 constraint system)
  - An R1CS is a sequence of groups of three vectors (a, b, c), and the solution to an R1CS is a vector s
  - s . a * s . b - s . c = 0, where . represents the dot product
