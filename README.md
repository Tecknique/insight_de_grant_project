### Project Idea
This project focuses on creating a low latency, scalable solution to provide fault tolerant, live  analytical data on present and historical federal government funding practices.

###  Tech Stack
Raw Data: usaspending.gov api

S3: to store the over 1 TB of data

Kafka Streams: Send data into a kafka cluster via its producer of topics and their partitions. Kafka runs on one or more broker (server) and the partitions of the topics are distributed out across the cluster nodes. Partitions are copied to multiple brokers, which means that not only one “messenger” is sending the message, but multiple brokers are. This makes it fault tolerant

 (as a distributed messaging system of unbounded flow of facts. No micro-batching. It’s per-record streaming. Fault tolerant, elastically scalable.)

Apache Airflow: Data updates once a day so real time processing isn't necessary

PostgreSQL:  Relational Database

PyGal: Analytics

### Data
Source: USAspending.gov
Size: 1-2 TB. Just over 1 TB in early 2018
Available: Downloaded, updates daily

### Engineering Challenge

Large scale, changing data, analytical processing.
User selection of variables

### Business  Value
Provides insight into how consumers should skew their product or word their applications in order to receive lucrative government funding

### MVP
Provides analytics and visualization of current and past and present (streaming) trends of approved government funding based on a user interface engine with choices of variables to compare.
