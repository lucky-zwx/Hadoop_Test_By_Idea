# Hadoop_Test_By_Idea
***依靠IDEA编辑器***
这是一个显示/input文件夹下文件的程序
Hadoop开发环境测试
在创建项目的时候选择Maven项目
最重要的是编写好这个文件
![kSP5lQ.png](https://s2.ax1x.com/2019/01/16/kSP5lQ.png)
## 下面给一个实例，注意的是这个地方<version>2.9.2</version>，里面的数值是你的Hadoop版本号，依据实际情况修改，由于刚刚学配置文件实在是太多太复杂，都是依据网上教程copy的，编辑好xml文件之后Idea会提示你更新，点下载就好！

```
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.cloudera.hadoop</groupId>
    <artifactId>bigdata</artifactId>
    <version>1.0-SNAPSHOT</version>

    <repositories>
        <repository>
            <id>cloudera</id>
            <url>https://repository.cloudera.com/artifactory/cloudera-repos/</url>
            <releases>
                <enabled>true</enabled>
            </releases>
            <snapshots>
                <enabled>false</enabled>
            </snapshots>
        </repository>
    </repositories>

    <properties>
        <cdh.version>2.6.0-cdh5.15.0</cdh.version>
    </properties>

    <dependencies>
        <dependency>
            <groupId>org.apache.hadoop</groupId>
            <artifactId>hadoop-common</artifactId>
            <version>2.9.2</version>
            <scope>provided</scope>
        </dependency>
        <dependency>
            <groupId>org.apache.hadoop</groupId>
            <artifactId>hadoop-core</artifactId>
            <version>2.9.2</version>
            <scope>provided</scope>
        </dependency>
        <dependency>
            <groupId>org.apache.hadoop</groupId>
            <artifactId>hadoop-hdfs</artifactId>
            <version>2.9.2</version>
            <scope>provided</scope>
        </dependency>
        <dependency>
            <groupId>org.apache.hadoop</groupId>
            <artifactId>hadoop-client</artifactId>
            <version>2.9.2</version>
            <scope>provided</scope>
        </dependency>
    </dependencies>
</project>

```
