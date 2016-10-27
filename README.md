# Apache Spark

## Installation

### Environment info     

OS

```
Mac OS X 10.12
```

Java

```shell
[anuragkapur@ak-skynet servers] $ java -version
java version "1.8.0_45"
Java(TM) SE Runtime Environment (build 1.8.0_45-b14)
Java HotSpot(TM) 64-Bit Server VM (build 25.45-b02, mixed mode)
```

Scala

```shell
[anuragkapur@ak-skynet servers] $ scala
Welcome to Scala version 2.11.7 (Java HotSpot(TM) 64-Bit Server VM, Java 1.8.0_45).
```    

### Steps
* Download from http://spark.apache.org/downloads.html
    File: spark-2.0.1-bin-hadoop2.7.tgz
* Unpack to a suitable dir
* Run an example to verify
```shell
$ ./bin/run-example SparkPi 10
```

Output (truncated)

```
...
16/10/23 22:12:30 INFO DAGScheduler: Job 0 finished: reduce at SparkPi.scala:38, took 1.086911 s
Pi is roughly 3.1435031435031435
16/10/23 22:12:30 INFO SparkUI: Stopped Spark web UI at http://192.168.1.67:4040
...
```

## Using Spark

### Spark shell

```shell
# The --master option specifies the master URL for a distributed cluster, or local to run locally with one thread,
# or local[N] to run locally with N threads.
$ ./bin/spark-shell --master local[2]
```

### Python interpreter

```shell
./bin/pyspark --master local[2]
```

### Quick start tutorial
[http://spark.apache.org/docs/latest/quick-start.html](http://spark.apache.org/docs/latest/quick-start.html)

### Spark programming guide
[http://spark.apache.org/docs/latest/programming-guide.html](http://spark.apache.org/docs/latest/programming-guide.html)

### Spark cluster mode
[http://spark.apache.org/docs/latest/cluster-overview.html](http://spark.apache.org/docs/latest/cluster-overview.html)
