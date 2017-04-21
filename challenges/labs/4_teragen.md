TERAGEN

[neymar@ip-172-31-48-240 root]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Dmapred.map.tasks=8 -Ddfs.block.size=16777216 65536000 /user/neymar/tgen640
17/04/20 22:25:38 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-57-83.ec2.internal/172.31.57.83:8032
17/04/20 22:25:39 INFO terasort.TeraGen: Generating 65536000 using 8
17/04/20 22:25:39 INFO mapreduce.JobSubmitter: number of splits:8
17/04/20 22:25:39 INFO Configuration.deprecation: mapred.map.tasks is deprecated. Instead, use mapreduce.job.maps
17/04/20 22:25:39 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/04/20 22:25:39 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492740334345_0001
17/04/20 22:25:40 INFO impl.YarnClientImpl: Submitted application application_1492740334345_0001
17/04/20 22:25:40 INFO mapreduce.Job: The url to track the job: http://ip-172-31-57-83.ec2.internal:8088/proxy/application_1492740334345_0001/
17/04/20 22:25:40 INFO mapreduce.Job: Running job: job_1492740334345_0001
17/04/20 22:25:48 INFO mapreduce.Job: Job job_1492740334345_0001 running in uber mode : false
17/04/20 22:25:48 INFO mapreduce.Job:  map 0% reduce 0%
17/04/20 22:26:07 INFO mapreduce.Job:  map 14% reduce 0%
17/04/20 22:26:08 INFO mapreduce.Job:  map 18% reduce 0%
17/04/20 22:26:09 INFO mapreduce.Job:  map 26% reduce 0%
17/04/20 22:26:14 INFO mapreduce.Job:  map 27% reduce 0%
17/04/20 22:26:16 INFO mapreduce.Job:  map 28% reduce 0%
17/04/20 22:26:20 INFO mapreduce.Job:  map 32% reduce 0%
17/04/20 22:26:22 INFO mapreduce.Job:  map 36% reduce 0%
17/04/20 22:26:26 INFO mapreduce.Job:  map 39% reduce 0%
17/04/20 22:26:28 INFO mapreduce.Job:  map 40% reduce 0%
17/04/20 22:26:32 INFO mapreduce.Job:  map 42% reduce 0%
17/04/20 22:26:34 INFO mapreduce.Job:  map 46% reduce 0%
17/04/20 22:26:38 INFO mapreduce.Job:  map 49% reduce 0%
17/04/20 22:26:40 INFO mapreduce.Job:  map 50% reduce 0%
17/04/20 22:26:44 INFO mapreduce.Job:  map 52% reduce 0%
17/04/20 22:26:46 INFO mapreduce.Job:  map 54% reduce 0%
17/04/20 22:26:50 INFO mapreduce.Job:  map 56% reduce 0%
17/04/20 22:26:56 INFO mapreduce.Job:  map 61% reduce 0%
17/04/20 22:26:57 INFO mapreduce.Job:  map 62% reduce 0%
17/04/20 22:26:58 INFO mapreduce.Job:  map 64% reduce 0%
17/04/20 22:27:02 INFO mapreduce.Job:  map 67% reduce 0%
17/04/20 22:27:04 INFO mapreduce.Job:  map 70% reduce 0%
17/04/20 22:27:08 INFO mapreduce.Job:  map 71% reduce 0%
17/04/20 22:27:10 INFO mapreduce.Job:  map 72% reduce 0%
17/04/20 22:27:14 INFO mapreduce.Job:  map 75% reduce 0%
17/04/20 22:27:15 INFO mapreduce.Job:  map 76% reduce 0%
17/04/20 22:27:16 INFO mapreduce.Job:  map 79% reduce 0%
17/04/20 22:27:18 INFO mapreduce.Job:  map 82% reduce 0%
17/04/20 22:27:22 INFO mapreduce.Job:  map 86% reduce 0%
17/04/20 22:27:26 INFO mapreduce.Job:  map 88% reduce 0%
17/04/20 22:27:32 INFO mapreduce.Job:  map 95% reduce 0%
17/04/20 22:27:35 INFO mapreduce.Job:  map 100% reduce 0%
17/04/20 22:27:36 INFO mapreduce.Job: Job job_1492740334345_0001 completed successfully
17/04/20 22:27:36 INFO mapreduce.Job: Counters: 33
        File System Counters
                FILE: Number of bytes read=0
                FILE: Number of bytes written=1019040
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=682
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=32
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=8
                Other local map tasks=8
                Total time spent by all maps in occupied slots (ms)=644576
                Total time spent by all reduces in occupied slots (ms)=0
                Total time spent by all map tasks (ms)=644576
                Total vcore-milliseconds taken by all map tasks=644576
                Total megabyte-milliseconds taken by all map tasks=660045824
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Input split bytes=682
                Spilled Records=0
                Failed Shuffles=0
                Merged Map outputs=0
                GC time elapsed (ms)=1745
                CPU time spent (ms)=137250
                Physical memory (bytes) snapshot=2805063680
                Virtual memory (bytes) snapshot=12622905344
                Total committed heap usage (bytes)=2881486848
                Peak Map Physical memory (bytes)=388771840
                Peak Map Virtual memory (bytes)=1591123968
        org.apache.hadoop.examples.terasort.TeraGen$Counters
                CHECKSUM=140750829423462787
        File Input Format Counters
                Bytes Read=0
        File Output Format Counters
                Bytes Written=6553600000

TIME

real    2m1.636s
user    0m6.157s
sys     0m0.292s

[neymar@ip-172-31-48-240 root]$ hdfs dfs -ls /user/neymar/tgen640
Found 9 items
-rw-r--r--   3 neymar merengues          0 2017-04-20 22:27 /user/neymar/tgen640/_SUCCESS
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00000
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00001
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00002
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00003
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00004
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00005
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00006
-rw-r--r--   3 neymar merengues  819200000 2017-04-20 22:27 /user/neymar/tgen640/part-m-00007


[neymar@ip-172-31-48-240 root]$ hdfs  fsck /user/neymar/tgen640 -blocks
Connecting to namenode via http://ip-172-31-57-83.ec2.internal:50070
FSCK started by neymar (auth:SIMPLE) from /172.31.48.240 for path /user/neymar/tgen640 at Thu Apr 20 22:29:37 EDT 2017
.........Status: HEALTHY
 Total size:    6553600000 B
 Total dirs:    1
 Total files:   9
 Total symlinks:                0
 Total blocks (validated):      392 (avg. block size 16718367 B)
 Minimally replicated blocks:   392 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Thu Apr 20 22:29:37 EDT 2017 in 14 milliseconds


The filesystem under path '/user/neymar/tgen640' is HEALTHY
[neymar@ip-172-31-48-240 root]$




