### Archetype simplewebapp
```bash
mvn archetype:generate -DgroupId=sample -DartifactId=maven-archetype-webapp-alpine -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false
```

### How to run
```bash
mvn clean package
docker run -p 8080:8080 -d maven-archetype-webapp-alpine
wget localhost:8080/maven-archetype-webapp-alpine/ && cat index.html
```