# reveal.js to map.apps jar

This project converts the reveal.js bower version to a map.apps friendly jar.

## Upgrade Instructions

1. update the version in bower.json

2. check .bowerrc and exclude all other dependencies

3. check the pom.xml for package.json manipulation

4. update the version of the pom.xml

5. execute mvn for testing output

        mvn clean package

6. execute mvn for upload to nexus

        mvn clean deploy -DupdateReleaseInfo=true
