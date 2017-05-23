# THEME GENERATION WITH MAVEN ARCHETYPE

### Example 1:

```bash
mvn archetype:generate -DarchetypeVersion=1.0.0-SNAPSHOT -DarchetypeGroupId=org.wso2.carbon.uuf.maven -DarchetypeArtifactId=uuf-theme-archetype 
```

will generate the app with default values...

* **groupId:** org.wso2.carbon.uuf
* **artifactId:** org.wso2.carbon.uuf.theme.default.theme
* **version:** 1.0.0-SNAPSHOT

### Example 2:

```bash
mvn archetype:generate -DarchetypeVersion=1.0.0-SNAPSHOT -DarchetypeGroupId=org.wso2.carbon.uuf.maven -DarchetypeArtifactId=uuf-theme-archetype -DgroupId=org.wso2.carbon.uuf.sample -DartifactId=org.wso2.carbon.uuf.sample.mytheme -Dversion=1.0.0-SNAPSHOT -Dpackage=org.wso2.carbon.uuf.sample.mytheme
```

will generate the app with...

* **groupId:** org.wso2.carbon.uuf.sample
* **artifactId:** org.wso2.carbon.uuf.sample.mytheme.theme
* **version:** 1.0.0-SNAPSHOT

# STRUCTURE OF THE THEME

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

