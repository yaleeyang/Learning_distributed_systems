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
    
    
    
