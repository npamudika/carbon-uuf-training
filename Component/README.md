# COMPONENT GENERATION WITH MAVEN ARCHETYPE

### Example 1:

```bash
mvn archetype:generate -DarchetypeVersion=1.0.0-SNAPSHOT -DarchetypeGroupId=org.wso2.carbon.uuf.maven -DarchetypeArtifactId=uuf-component-archetype 
```

will generate the app with default values...

* **groupId:** org.wso2.carbon.uuf.sample
* **artifactId:** org.wso2.carbon.uuf.sample.hello-world.ui
* **version:** 1.0.0-SNAPSHOT
* **package:** org.wso2.carbon.uuf.sample.hello-world.ui
* **componentName:** Hello World Component


### Example 2:

```bash
mvn archetype:generate -DarchetypeVersion=1.0.0-SNAPSHOT -DarchetypeGroupId=org.wso2.carbon.uuf.maven -DarchetypeArtifactId=uuf-component-archetype -DgroupId=org.wso2.carbon.uuf.sample -DartifactId=org.wso2.carbon.uuf.sample.mycomponent -Dversion=1.0.0-SNAPSHOT -DcomponentName=My\ Component
```

will generate the app with...

* **groupId:** org.wso2.carbon.uuf.sample
* **artifactId:** org.wso2.carbon.uuf.sample.mycomponent.ui
* **version:** 1.0.0-SNAPSHOT
* **package:** org.wso2.carbon.uuf.sample.mycomponent.ui
* **componentName:** My Component

# STRUCTURE OF THE COMPONENT

```
  org.wso2.carbon.<product-name>.<component-name>
|----src
|    |----main
|         |----pages
|         |
|         |----layouts
|         |
|         |----fragments
|         |
|         |----modules
|         |
|         |----lang
|         |
|         |----public
|         |
|         ‘---- component.yaml
|
‘---- pom.xml

```

