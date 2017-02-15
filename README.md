# Assignment-2.2
1) HDFS
• The file store in HDFS provides scalable, fault-tolerant storage at low cost.
• The HDFS software detects and compensates for hardware issues, including disk problems and server failure.
• HDFS stores files across the collection of servers in a cluster.
• Files are decomposed into blocks and each block is written to more than one of the servers.
• The replication provides both fault-tolerance and performance.

The Design of HDFS
• Very large files: Files that are megabytes, gigabytes, terabytes, or petabytes of size.
• Streaming data access: HDFS is built around the idea that data is written once but read many times. A dataset is copied from source and then analysis is done on that dataset over time.
• Commodity hardware: Hadoop does not require expensive, highly reliable hardware as it is designed to run on clusters of commodity hardware.

2)Hadoop cluster
A Hadoop cluster is a special type of computational cluster designed specifically for storing and analyzing huge amounts of unstructured data in a distributed computing environment. Such clusters run Hadoop's open source distributed processing software on low-cost commodity computers. Typically one machine in the cluster is designated as the NameNode and another machine the as JobTracker; these are the masters. The rest of the machines in the cluster act as both DataNode and TaskTracker; these are the slaves. Hadoop clusters are often referred to as "shared nothing" systems because the only thing that is shared between nodes is the network that connects them.Hadoop clusters are known for boosting the speed of data analysis applications. 

3)HDFS blocks
•A Hard Disk has concentric circles which form tracks.
• One file can contain many blocks. These blocks in a local file system are nearly 512 bytes and are not necessarily continuous.
• For HDFS, since it is designed for large files, the block size is 128 MB by default. Moreover, it gets blocks of local file system contiguously to minimise the head seek time.
