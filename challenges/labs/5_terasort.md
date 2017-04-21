[root@ip-172-31-63-59 ~]# kinit neymar
Password for neymar@FABIOMMFF.BR:
[root@ip-172-31-63-59 ~]# hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort tgen640 tsort640m
17/04/20 23:44:45 INFO terasort.TeraSort: starting
17/04/20 23:44:47 INFO hdfs.DFSClient: Created token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@FABIOMMFF.BR, renewer=yarn, realUser=, issueDate=1492746287162, maxDate=1493351087162, sequenceNumber=1, masterKeyId=2 on 172.31.57.83:8020
17/04/20 23:44:47 INFO security.TokenCache: Got dt for hdfs://ip-172-31-57-83.ec2.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.57.83:8020, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@FABIOMMFF.BR, renewer=yarn, realUser=, issueDate=1492746287162, maxDate=1493351087162, sequenceNumber=1, masterKeyId=2)
17/04/20 23:44:47 INFO input.FileInputFormat: Total input paths to process : 8
Spent 464ms computing base-splits.
Spent 7ms computing TeraScheduler splits.
Computing input splits took 472ms
Sampling 10 splits of 392
Making 8 from 100000 sampled records
Computing parititions took 867ms
Spent 1341ms computing partitions.
17/04/20 23:44:48 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-57-83.ec2.internal/172.31.57.83:8032
17/04/20 23:44:48 INFO mapreduce.JobSubmitter: number of splits:392
17/04/20 23:44:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492745807062_0001
17/04/20 23:44:49 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.57.83:8020, Ident: (token for neymar: HDFS_DELEGATION_TOKEN owner=neymar@FABIOMMFF.BR, renewer=yarn, realUser=, issueDate=1492746287162, maxDate=1493351087162, sequenceNumber=1, masterKeyId=2)
17/04/20 23:44:50 INFO impl.YarnClientImpl: Submitted application application_1492745807062_0001
17/04/20 23:44:50 INFO mapreduce.Job: The url to track the job: http://ip-172-31-57-83.ec2.internal:8088/proxy/application_1492745807062_0001/
17/04/20 23:44:50 INFO mapreduce.Job: Running job: job_1492745807062_0001
17/04/20 23:45:01 INFO mapreduce.Job: Job job_1492745807062_0001 running in uber mode : false
17/04/20 23:45:01 INFO mapreduce.Job:  map 0% reduce 0%
17/04/20 23:45:13 INFO mapreduce.Job:  map 1% reduce 0%
17/04/20 23:45:18 INFO mapreduce.Job:  map 2% reduce 0%
17/04/20 23:45:20 INFO mapreduce.Job:  map 3% reduce 0%
17/04/20 23:45:27 INFO mapreduce.Job:  map 4% reduce 0%
17/04/20 23:45:28 INFO mapreduce.Job:  map 5% reduce 0%
17/04/20 23:45:35 INFO mapreduce.Job:  map 6% reduce 0%
17/04/20 23:45:42 INFO mapreduce.Job:  map 7% reduce 0%
17/04/20 23:45:46 INFO mapreduce.Job:  map 8% reduce 0%
17/04/20 23:45:49 INFO mapreduce.Job:  map 9% reduce 0%
17/04/20 23:45:55 INFO mapreduce.Job:  map 10% reduce 0%
17/04/20 23:45:57 INFO mapreduce.Job:  map 11% reduce 0%
17/04/20 23:46:04 INFO mapreduce.Job:  map 12% reduce 0%
17/04/20 23:46:06 INFO mapreduce.Job:  map 13% reduce 0%
17/04/20 23:46:10 INFO mapreduce.Job:  map 14% reduce 0%
17/04/20 23:46:15 INFO mapreduce.Job:  map 15% reduce 0%
17/04/20 23:46:18 INFO mapreduce.Job:  map 16% reduce 0%
17/04/20 23:46:24 INFO mapreduce.Job:  map 17% reduce 0%
17/04/20 23:46:29 INFO mapreduce.Job:  map 18% reduce 0%
17/04/20 23:46:32 INFO mapreduce.Job:  map 19% reduce 0%
17/04/20 23:46:37 INFO mapreduce.Job:  map 20% reduce 0%
17/04/20 23:46:41 INFO mapreduce.Job:  map 21% reduce 0%
17/04/20 23:46:46 INFO mapreduce.Job:  map 22% reduce 0%
17/04/20 23:46:52 INFO mapreduce.Job:  map 23% reduce 0%
17/04/20 23:46:54 INFO mapreduce.Job:  map 24% reduce 0%
17/04/20 23:47:00 INFO mapreduce.Job:  map 25% reduce 0%
17/04/20 23:47:02 INFO mapreduce.Job:  map 26% reduce 0%
17/04/20 23:47:07 INFO mapreduce.Job:  map 27% reduce 0%
17/04/20 23:47:12 INFO mapreduce.Job:  map 28% reduce 0%
17/04/20 23:47:18 INFO mapreduce.Job:  map 29% reduce 0%
17/04/20 23:47:21 INFO mapreduce.Job:  map 30% reduce 0%
17/04/20 23:47:27 INFO mapreduce.Job:  map 31% reduce 0%
17/04/20 23:47:32 INFO mapreduce.Job:  map 32% reduce 0%
17/04/20 23:47:34 INFO mapreduce.Job:  map 33% reduce 0%
17/04/20 23:47:41 INFO mapreduce.Job:  map 34% reduce 0%
17/04/20 23:47:42 INFO mapreduce.Job:  map 35% reduce 0%
17/04/20 23:47:50 INFO mapreduce.Job:  map 36% reduce 0%
17/04/20 23:47:53 INFO mapreduce.Job:  map 37% reduce 0%
17/04/20 23:47:56 INFO mapreduce.Job:  map 38% reduce 0%
17/04/20 23:48:02 INFO mapreduce.Job:  map 39% reduce 0%
17/04/20 23:48:08 INFO mapreduce.Job:  map 40% reduce 0%
17/04/20 23:48:15 INFO mapreduce.Job:  map 41% reduce 0%
17/04/20 23:48:17 INFO mapreduce.Job:  map 42% reduce 0%
17/04/20 23:48:23 INFO mapreduce.Job:  map 43% reduce 0%
17/04/20 23:48:27 INFO mapreduce.Job:  map 44% reduce 0%
17/04/20 23:48:32 INFO mapreduce.Job:  map 45% reduce 0%
17/04/20 23:48:36 INFO mapreduce.Job:  map 46% reduce 0%
17/04/20 23:48:43 INFO mapreduce.Job:  map 47% reduce 0%
17/04/20 23:48:44 INFO mapreduce.Job:  map 48% reduce 0%
17/04/20 23:48:50 INFO mapreduce.Job:  map 49% reduce 0%
17/04/20 23:48:53 INFO mapreduce.Job:  map 50% reduce 0%
17/04/20 23:48:57 INFO mapreduce.Job:  map 51% reduce 0%
17/04/20 23:49:03 INFO mapreduce.Job:  map 52% reduce 0%
17/04/20 23:49:05 INFO mapreduce.Job:  map 53% reduce 0%
17/04/20 23:49:12 INFO mapreduce.Job:  map 54% reduce 0%
17/04/20 23:49:15 INFO mapreduce.Job:  map 55% reduce 0%
17/04/20 23:49:21 INFO mapreduce.Job:  map 56% reduce 0%
17/04/20 23:49:24 INFO mapreduce.Job:  map 57% reduce 0%
17/04/20 23:49:31 INFO mapreduce.Job:  map 58% reduce 0%
17/04/20 23:49:33 INFO mapreduce.Job:  map 59% reduce 0%
17/04/20 23:49:39 INFO mapreduce.Job:  map 60% reduce 0%
17/04/20 23:49:42 INFO mapreduce.Job:  map 61% reduce 0%
17/04/20 23:49:47 INFO mapreduce.Job:  map 62% reduce 0%
17/04/20 23:49:51 INFO mapreduce.Job:  map 63% reduce 0%
17/04/20 23:49:54 INFO mapreduce.Job:  map 64% reduce 0%
17/04/20 23:50:01 INFO mapreduce.Job:  map 65% reduce 0%
17/04/20 23:50:04 INFO mapreduce.Job:  map 66% reduce 0%
17/04/20 23:50:11 INFO mapreduce.Job:  map 67% reduce 0%
17/04/20 23:50:12 INFO mapreduce.Job:  map 68% reduce 0%
17/04/20 23:50:19 INFO mapreduce.Job:  map 69% reduce 0%
17/04/20 23:50:21 INFO mapreduce.Job:  map 70% reduce 0%
17/04/20 23:50:29 INFO mapreduce.Job:  map 71% reduce 0%
17/04/20 23:50:32 INFO mapreduce.Job:  map 72% reduce 0%
17/04/20 23:50:37 INFO mapreduce.Job:  map 73% reduce 0%
17/04/20 23:50:41 INFO mapreduce.Job:  map 74% reduce 0%
17/04/20 23:50:47 INFO mapreduce.Job:  map 75% reduce 0%
17/04/20 23:50:49 INFO mapreduce.Job:  map 76% reduce 0%
17/04/20 23:50:53 INFO mapreduce.Job:  map 77% reduce 0%
17/04/20 23:50:58 INFO mapreduce.Job:  map 78% reduce 0%
17/04/20 23:51:01 INFO mapreduce.Job:  map 79% reduce 0%
17/04/20 23:51:08 INFO mapreduce.Job:  map 80% reduce 0%
17/04/20 23:51:10 INFO mapreduce.Job:  map 81% reduce 0%
17/04/20 23:51:17 INFO mapreduce.Job:  map 82% reduce 0%
17/04/20 23:51:21 INFO mapreduce.Job:  map 83% reduce 0%
17/04/20 23:51:28 INFO mapreduce.Job:  map 83% reduce 3%
17/04/20 23:51:33 INFO mapreduce.Job:  map 83% reduce 7%
17/04/20 23:51:35 INFO mapreduce.Job:  map 84% reduce 10%
17/04/20 23:51:39 INFO mapreduce.Job:  map 84% reduce 14%
17/04/20 23:51:46 INFO mapreduce.Job:  map 85% reduce 14%
17/04/20 23:51:54 INFO mapreduce.Job:  map 86% reduce 14%
17/04/20 23:52:01 INFO mapreduce.Job:  map 87% reduce 14%
17/04/20 23:52:08 INFO mapreduce.Job:  map 88% reduce 14%
17/04/20 23:52:09 INFO mapreduce.Job:  map 88% reduce 15%
17/04/20 23:52:15 INFO mapreduce.Job:  map 89% reduce 15%
17/04/20 23:52:25 INFO mapreduce.Job:  map 90% reduce 15%
17/04/20 23:52:37 INFO mapreduce.Job:  map 91% reduce 15%
17/04/20 23:52:44 INFO mapreduce.Job:  map 92% reduce 15%
17/04/20 23:52:51 INFO mapreduce.Job:  map 93% reduce 15%
17/04/20 23:53:00 INFO mapreduce.Job:  map 94% reduce 15%
17/04/20 23:53:03 INFO mapreduce.Job:  map 94% reduce 16%
17/04/20 23:53:12 INFO mapreduce.Job:  map 95% reduce 16%
17/04/20 23:53:21 INFO mapreduce.Job:  map 96% reduce 16%
17/04/20 23:53:29 INFO mapreduce.Job:  map 97% reduce 16%
17/04/20 23:53:37 INFO mapreduce.Job:  map 98% reduce 16%
17/04/20 23:53:47 INFO mapreduce.Job:  map 99% reduce 16%
17/04/20 23:53:53 INFO mapreduce.Job:  map 99% reduce 17%
17/04/20 23:53:55 INFO mapreduce.Job:  map 100% reduce 17%
17/04/20 23:54:03 INFO mapreduce.Job:  map 100% reduce 26%
17/04/20 23:54:04 INFO mapreduce.Job:  map 100% reduce 31%
17/04/20 23:54:05 INFO mapreduce.Job:  map 100% reduce 36%
17/04/20 23:54:08 INFO mapreduce.Job:  map 100% reduce 40%
17/04/20 23:54:09 INFO mapreduce.Job:  map 100% reduce 44%
17/04/20 23:54:10 INFO mapreduce.Job:  map 100% reduce 47%
17/04/20 23:54:11 INFO mapreduce.Job:  map 100% reduce 49%
17/04/20 23:54:12 INFO mapreduce.Job:  map 100% reduce 53%
17/04/20 23:54:13 INFO mapreduce.Job:  map 100% reduce 56%
17/04/20 23:54:14 INFO mapreduce.Job:  map 100% reduce 61%
17/04/20 23:54:15 INFO mapreduce.Job:  map 100% reduce 62%
17/04/20 23:54:16 INFO mapreduce.Job:  map 100% reduce 66%
17/04/20 23:54:18 INFO mapreduce.Job:  map 100% reduce 71%
17/04/20 23:54:22 INFO mapreduce.Job:  map 100% reduce 73%
17/04/20 23:54:23 INFO mapreduce.Job:  map 100% reduce 78%
17/04/20 23:54:25 INFO mapreduce.Job:  map 100% reduce 81%
17/04/20 23:54:28 INFO mapreduce.Job:  map 100% reduce 82%
17/04/20 23:54:29 INFO mapreduce.Job:  map 100% reduce 86%
17/04/20 23:54:30 INFO mapreduce.Job:  map 100% reduce 90%
17/04/20 23:54:36 INFO mapreduce.Job:  map 100% reduce 94%
17/04/20 23:54:42 INFO mapreduce.Job:  map 100% reduce 98%
17/04/20 23:54:45 INFO mapreduce.Job:  map 100% reduce 100%
17/04/20 23:54:46 INFO mapreduce.Job: Job job_1492745807062_0001 completed successfully
17/04/20 23:54:46 INFO mapreduce.Job: Counters: 54
        File System Counters
                FILE: Number of bytes read=2909525381
                FILE: Number of bytes written=5804559960
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=6553654096
                HDFS: Number of bytes written=6553600000
                HDFS: Number of read operations=1200
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=16
        Job Counters
                Launched map tasks=392
                Launched reduce tasks=8
                Data-local map tasks=390
                Rack-local map tasks=2
                Total time spent by all maps in occupied slots (ms)=2632809
                Total time spent by all reduces in occupied slots (ms)=840199
                Total time spent by all map tasks (ms)=2632809
                Total time spent by all reduce tasks (ms)=840199
                Total vcore-milliseconds taken by all map tasks=2632809
                Total vcore-milliseconds taken by all reduce tasks=840199
                Total megabyte-milliseconds taken by all map tasks=2695996416
                Total megabyte-milliseconds taken by all reduce tasks=860363776
        Map-Reduce Framework
                Map input records=65536000
                Map output records=65536000
                Map output bytes=6684672000
                Map output materialized bytes=2843187873
                Input split bytes=54096
                Combine input records=0
                Combine output records=0
                Reduce input groups=65536000
                Reduce shuffle bytes=2843187873
                Reduce input records=65536000
                Reduce output records=65536000
                Spilled Records=131072000
                Shuffled Maps =3136
                Failed Shuffles=0
                Merged Map outputs=3136
                GC time elapsed (ms)=33740
                CPU time spent (ms)=1466710
                Physical memory (bytes) snapshot=188827688960
                Virtual memory (bytes) snapshot=632017297408
                Total committed heap usage (bytes)=224619134976
                Peak Map Physical memory (bytes)=508821504
                Peak Map Virtual memory (bytes)=1593352192
                Peak Reduce Physical memory (bytes)=983810048
                Peak Reduce Virtual memory (bytes)=1608773632
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=6553600000
        File Output Format Counters
                Bytes Written=6553600000
17/04/20 23:54:46 INFO terasort.TeraSort: done
[root@ip-172-31-63-59 ~]#
