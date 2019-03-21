### Project Idea
This project focuses on creating a low latency, scalable solution to provide fault tolerant, schedule-updated analytical data on present and historical federal government funding practices.

###  Tech Stack
Raw Data: usaspending.gov api

S3: to store the over 1 TB of data

Kafka: Fault tolerant storage, perform batch processing, best for managing large amounts of data.

 (as a distributed messaging system of unbounded flow of facts. No micro-batching. It’s per-record streaming. Fault tolerant, elastically scalable.)

Apache Airflow: Because new data is updated once a day, Apache Airflow is a better choice than Spark Streams or Apache Storm because you can set a timed update schedule.

PostgreSQL: Relational Database
or
SQLAlchemy: Python SQL toolkit

PyGal: Interactive visualizations

flask: web app toolkit



PyGal: Analytics

### Data
Source: USAspending.gov
Size: 1-2 TB. Just over 1 TB in early 2018
Available: Downloaded, updates daily

### Engineering Challenge

Large scale, scheduled updates of data, analytical processing.
User selection of variables

### Business  Value
Provides insight into how consumers should skew their product or word their applications in order to receive lucrative government funding

### MVP
Provides analytics and visualization of current and past and present (streaming) trends of approved government funding based on a user interface engine with choices of variables to compare.

### Stretch Goals
Join with databases that contain associated budgets, and IPO stocks stock market value after approval
