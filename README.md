# Hadoop DataNodeManger
Modified DataNodeManager for managing Hadoop cluster

1.   $HADOOP_SRC_HOME/hadoop-hdfs-project/hadoop-hdfs/src/main/java/org/apache/hadoop/hdfs/server/blockmanagement/DatanodeManager.java 의
파일을 본 프로그램의 소스코드로 변경
2. hadoop-common-project/hadoop-common/src/main/java/org/apache/hadoop/net/NetworkTopology.java  파일 본 프로그램의 소스코드로 변경
3. add dependency about hadoop-hdfs to pom.xml hadoop-common-project/hadoop-common project
4.   $HADOOP_SRC_HOME에서 Hadoop을 기존의 방법과 동일하게 컴파일 수행
($mvn package -Pdist -DskipTests –Dtar)
5.   hadoop-disk/target 에 생성된 binary로 HDFS 데몬을 실행
6.   hdfs dfsadmin –setStoragePolicy 명령을 통해 사용할 storage policy를 설정하여 사용

@성균관대학교 VLDB 연구실 (이상원 교수님) 
@담당연구원: 이종백
