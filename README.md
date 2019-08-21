Example Project for Okta's Maven Plugin
=======================================

## Prerequisite

- Java 8

## Get started 

Clone this repo:

```bash
# clone
git clone https://github.com/bdemers/spring-boot-demo-app.git
cd spring-boot-demo-app

# register for Free Okta Developer account, and setup this application
./mvnw com.okta:okta-maven-plugin:init

# start the application
./mvnw spring-boot:run

# browse to http://localhost:8080
```

Check your email for account activation information

## Future

After the first release of the plugin you can create a project using start.spring.io

If you _really_ want to do that now, you can add the following `pluginRepositories` block to your `pom.xml`

```xml
<pluginRepositories>
    <pluginRepository>
        <id>ossrh</id>
        <releases><enabled>false</enabled></releases>
        <snapshots><enabled>true</enabled></snapshots>
        <url>https://oss.sonatype.org/content/repositories/snapshots</url>
    </pluginRepository>
</pluginRepositories>
```