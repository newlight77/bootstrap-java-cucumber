# Bootstrap Java with Cucumber

This serves as a bootstrap for a basic Java Application integrating Cucumber.

## Run it

__Using Maven :__

```
mvn clean test
mvn clean verify -DCucumberOptions="--glue 'gradle.cucumber' --plugin pretty 'src/test/resources'"
mvn package
java -jar target/bootstrap-1.0.0-SNAPSHOT.jar MainApp ./data
```

__Using Gradle :__

```
gradle test
gradle cucumber
gradle build
java -jar libs/bootstrap-1.0.0-SNAPSHOT.jar MainApp ./data
```
