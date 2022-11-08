# -Java-word-count-beam
1. For checking maven version
mvn -v.

2. For creating word count folder
mvn archetype:generate `
-D archetypeGroupId=org.apache.beam `
-D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
-D archetypeVersion=2.42.0 `
-D groupId=org.example `
-D artifactId=word-count-beam `
-D version="0.1" `
-D package=org.apache.beam.examples `
-D interactiveMode=false

3. For changing directory
cd .\word-count-beam

4. To run a pipeline
mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
-D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner

5. For outputs
more counts*
