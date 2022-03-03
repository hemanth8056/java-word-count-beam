# java-word-count-beam
# Hemanth Venkata Reddy Telluri

## A sample wordcount eample pipeline using apache beam Java SDK

### To Check  java verion use
java --version

### To check the maven verion 
maven --version

### Generate a maven project using following command
mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false

 ### Run word count using maven 
mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
-D exec.args="--inputFile=sample.txt --output=telluri_output" -P direct-runner

