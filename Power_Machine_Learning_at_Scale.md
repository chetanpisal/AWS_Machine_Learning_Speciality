## Power Machine Learning at Scale

When you perform deep learning (DL) at scale, for example, datasets are commonly too large to fit into memory and therefore require pre-processing steps to partition the datasets. 


In general, 

a best practice is to pack the data in parallel, distributed across multiple machines. You should do this in a single run, and 

split the data into a small number of files with a uniform number of partitions. When the data is partitioned, it is readily accessible and easily fed in as batches across multiple machines. 

When the data is split into a small number of files, the preparation job can be parallelized and thus run faster. You can do all of this using frameworks such as MapReduce and Apache Spark. Running an Apache Spark cluster on Amazon EMR provides a managed framework that can process massive quantities of data.

