# JMH-Benchmark

**1. JMH(Java Microbenchmark Harness)**

: Java 성능분석을 위한 툴

참고 URL : http://tutorials.jenkov.com/java-performance/jmh.html

**2. 설치방법**

1) https://maven.apache.org/ 접속해서 MAVEN 설치
2) Maven 설치폴더를 Path에 등록
   ex) C:\apache-maven-3.6.3\bin
3) Command창에서 "mvn -version"을 입력하여 Maven 정상 설치 확인
4) 하기 명령어를 command창에서 수행
```
$ mvn archetype:generate -DinteractiveMode=false -DarchetypeGroupId=org.openjdk.jmh -DarchetypeArtifactId=jmh-java-benchmark-archetype -DgroupId=com.redrabbit88.sample -DartifactId=jmh-sample -Dversion=1
// -DgroupId=com.redrabbit88.sample
// 생성하는 패키지명을 결정함.
```
5) JMH을 사용하는 프로젝트가 생성됨.

**3. 실행방법**

1) JMH를 이용하도록 자바 소스 작성
2) **Maven Build**를 이용해서 빌드 수행
3) Command창을 이용해서 관련 프로젝트 위치로 이동
4) 하기 명령어를 command창에서 수행
```
$ mvn clean install
$ java -jar target/benchmarks.jar
// benchmarks.jar : JMH를 이용해서 생성되는 JAR 파일
```
