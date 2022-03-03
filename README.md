# java-word-count-beam by Rohit Reddy Chandupatla


### Use the following command to generate a Maven project that contains Beam’s WordCount examples and builds against the most recent Beam release:
### All of these commands should be run in Powershell.

```
mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false

```
### Get sample text

In the word-count-beam directory, create a file called [sample.txt.](https://github.com/RohitChandupatla/java-word-count-beam/blob/main/sample.txt)

### Run WordCount Using Maven For Windows PowerShell:
```
mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
``` 
