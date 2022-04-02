# azure-tomcat-webapp

### Create Project from Maven Architype
mvn archetype:generate "-DgroupId=com.skt.webapp" "-DartifactId=app01" "-DarchetypeArtifactId=maven-archetype-webapp" "-Dversion=1.0"

### Configure Project
mvn com.microsoft.azure:azure-webapp-maven-plugin:2.5.0:config

### Build & Deploy
mvn clean package
mvn package azure-webapp:deploy

### References:
- https://docs.microsoft.com/en-gb/azure/app-service/quickstart-java?pivots=platform-linux&tabs=tomcat
