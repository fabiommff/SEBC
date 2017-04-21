[root@ip-172-31-63-59 ~]# kinit ronaldo
Password for ronaldo@FABIOMMFF.BR:
[root@ip-172-31-63-59 ~]# hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar pi 8 2048
Number of Maps  = 8
Samples per Map = 2048
Wrote input for Map #0
Wrote input for Map #1
Wrote input for Map #2
Wrote input for Map #3
Wrote input for Map #4
Wrote input for Map #5
Wrote input for Map #6
Wrote input for Map #7
Starting Job
17/04/20 23:56:39 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-57-83.ec2.internal/172.31.57.83:8032
17/04/20 23:56:39 INFO hdfs.DFSClient: Created token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@FABIOMMFF.BR, renewer=yarn, realUser=, issueDate=1492746999731, maxDate=1493351799731, sequenceNumber=2, masterKeyId=2 on 172.31.57.83:8020
17/04/20 23:56:39 INFO security.TokenCache: Got dt for hdfs://ip-172-31-57-83.ec2.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.57.83:8020, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@FABIOMMFF.BR, renewer=yarn, realUser=, issueDate=1492746999731, maxDate=1493351799731, sequenceNumber=2, masterKeyId=2)
17/04/20 23:56:39 INFO input.FileInputFormat: Total input paths to process : 8
17/04/20 23:56:39 INFO mapreduce.JobSubmitter: number of splits:8
17/04/20 23:56:40 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1492745807062_0002
17/04/20 23:56:40 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.57.83:8020, Ident: (token for ronaldo: HDFS_DELEGATION_TOKEN owner=ronaldo@FABIOMMFF.BR, renewer=yarn, realUser=, issueDate=1492746999731, maxDate=1493351799731, sequenceNumber=2, masterKeyId=2)
17/04/20 23:56:40 INFO impl.YarnClientImpl: Submitted application application_1492745807062_0002
17/04/20 23:56:40 INFO mapreduce.Job: The url to track the job: http://ip-172-31-57-83.ec2.internal:8088/proxy/application_1492745807062_0002/
17/04/20 23:56:40 INFO mapreduce.Job: Running job: job_1492745807062_0002
17/04/20 23:56:49 INFO mapreduce.Job: Job job_1492745807062_0002 running in uber mode : false
17/04/20 23:56:49 INFO mapreduce.Job:  map 0% reduce 0%
17/04/20 23:57:00 INFO mapreduce.Job:  map 25% reduce 0%
17/04/20 23:57:01 INFO mapreduce.Job:  map 50% reduce 0%
17/04/20 23:57:03 INFO mapreduce.Job:  map 75% reduce 0%
17/04/20 23:57:04 INFO mapreduce.Job:  map 88% reduce 0%
17/04/20 23:57:05 INFO mapreduce.Job:  map 100% reduce 0%
17/04/20 23:57:10 INFO mapreduce.Job:  map 100% reduce 100%
17/04/20 23:57:10 INFO mapreduce.Job: Job job_1492745807062_0002 completed successfully
17/04/20 23:57:10 INFO mapreduce.Job: Counters: 53
        File System Counters
                FILE: Number of bytes read=81
                FILE: Number of bytes written=1159677
                FILE: Number of read operations=0
                FILE: Number of large read operations=0
                FILE: Number of write operations=0
                HDFS: Number of bytes read=2280
                HDFS: Number of bytes written=215
                HDFS: Number of read operations=35
                HDFS: Number of large read operations=0
                HDFS: Number of write operations=3
        Job Counters
                Launched map tasks=8
                Launched reduce tasks=1
                Data-local map tasks=8
                Total time spent by all maps in occupied slots (ms)=72893
                Total time spent by all reduces in occupied slots (ms)=3677
                Total time spent by all map tasks (ms)=72893
                Total time spent by all reduce tasks (ms)=3677
                Total vcore-milliseconds taken by all map tasks=72893
                Total vcore-milliseconds taken by all reduce tasks=3677
                Total megabyte-milliseconds taken by all map tasks=74642432
                Total megabyte-milliseconds taken by all reduce tasks=3765248
        Map-Reduce Framework
                Map input records=8
                Map output records=16
                Map output bytes=144
                Map output materialized bytes=280
                Input split bytes=1336
                Combine input records=0
                Combine output records=0
                Reduce input groups=2
                Reduce shuffle bytes=280
                Reduce input records=16
                Reduce output records=0
                Spilled Records=32
                Shuffled Maps =8
                Failed Shuffles=0
                Merged Map outputs=8
                GC time elapsed (ms)=481
                CPU time spent (ms)=6780
                Physical memory (bytes) snapshot=3821449216
                Virtual memory (bytes) snapshot=14261084160
                Total committed heap usage (bytes)=4580179968
                Peak Map Physical memory (bytes)=455987200
                Peak Map Virtual memory (bytes)=1591320576
                Peak Reduce Physical memory (bytes)=191258624
                Peak Reduce Virtual memory (bytes)=1601806336
        Shuffle Errors
                BAD_ID=0
                CONNECTION=0
                IO_ERROR=0
                WRONG_LENGTH=0
                WRONG_MAP=0
                WRONG_REDUCE=0
        File Input Format Counters
                Bytes Read=944
        File Output Format Counters
                Bytes Written=97
Job Finished in 30.682 seconds
Estimated value of Pi is 3.14111328125000000000
[root@ip-172-31-63-59 ~]#
