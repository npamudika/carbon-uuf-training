# APP GENERATION WITH MAVEN ARCHETYPE

### Example 1:

```bash
mvn archetype:generate -DarchetypeVersion=1.0.0-SNAPSHOT -DarchetypeGroupId=org.wso2.carbon.uuf.maven -DarchetypeArtifactId=uuf-app-archetype
```

will generate the app with default values...

**groupId:** org.wso2.carbon.uuf.sample
**artifactId:** org.wso2.carbon.uuf.sample.hello-world.feature
**version:** 1.0.0-SNAPSHOT
**package:** org.wso2.carbon.uuf.sample
**directoryName:** org.wso2.carbon.uuf.sample.hello-world.app

### Example 2:

```bash
mvn archetype:generate -DarchetypeVersion=1.0.0-SNAPSHOT -DarchetypeGroupId=org.wso2.carbon.uuf.maven -DarchetypeArtifactId=uuf-app-archetype -DgroupId=org.wso2.carbon.uuf.sample -DartifactId=org.wso2.carbon.uuf.sample.myapp.feature -Dversion=1.0.0-SNAPSHOT -DdirectoryName=org.wso2.carbon.uuf.sample.myapp.app
```

will generate the app with...

**groupId:** org.wso2.carbon.uuf.sample
**artifactId:** org.wso2.carbon.uuf.sample.myapp.feature
**version:** 1.0.0-SNAPSHOT
**package:** org.wso2.carbon.uuf.sample.myapp
**directoryName:** org.wso2.carbon.uuf.sample.myapp.app

##### Note:

Please note that the -DartifactId should end with “.feature” since upon building this will be created as a Carbon Feature

# STRUCTURE OF THE APP

```
org.wso2.carbon.<product-name>.<app-name>.feature
     |----src
     |     |----main
     |           |---- pages/
     |           |
     |           |---- fragments/
     |           |
     |           |---- layouts/
     |           |
     |           |---- modules/
     |           |
     |           |---- lang/
     |           |
     |           |---- public/
     |           |
     |           |---- app.yaml
     |           |
     |           ‘---- component.yaml
     ‘---- pom.xml

```

