# Haddop Key XML's Files.

## Installing Hadoop on local is easy task whereas configuring .XMLs is tedious.
###### I have configured .XMLs after debugging harshly and made it perfect which runs in a shot. However, I have done configurations after installing Hadoop 3.2.1 on MAC OSX.

###### Let's Begin with steps from the root:
1) Install Hadoop on system by using command: ` brew install hadoop`
2) Configure hadoop environment in ~./bashrc or ~./profile
3) Check Hadoop installed properly or not by command `hadoop version` and it should display Hadoop version `Hadoop x.x.x`
4) Clone this repo anywhere on local machine by using command: `git clone <repo link.git>`
5) Go to `/usr/local/Cellar/hadoop/3.2.1/libexec/etc/hadoop/`
6) You can see 
- core-site.xml
- hadoop-env.sh
- hdfs-site.xml
- mapred-env.sh
- mapred-site.xml
7) Finally replace above mentioned files with cloned files. That's it and you're done with the Job!!!
8) Head to terminal give command `cd /usr/local/Cellar/hadoop/3.2.1/sbin/`
9) You can see various files named as start-dfs.sh, stop-dfs.sh, start-all.sh stop-all.sh.
10) Now give command `./start-all.sh` to start hadoop all service on your local machine.
11) After start of DataNode, NameNode and ResourceManager kindly give command `hdfs dfs -ls /` to see hdfs directory.
- drwxrwxr-x   - satyamramawat supergroup          0 2019-10-26 01:59 /tmp
- drwx-wx-wx   - satyamramawat supergroup          0 2019-10-29 14:17 /user
12) Now lets check hadoop is working properly or not, so we can try some operational commands on hadoop like creating directory on HDFS (Hadoop Distributed File System) `hdfs dfs -mkdir /TestDirectory`
13) This command should create a directory and it will, if you had:
- [x] Installed hadoop properly.
- [x] Copied Pasted cloned file properly.


Author - Satyam Ramawat
