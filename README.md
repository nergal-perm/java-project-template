# Simple java project template archetype

This is a simple Java Maven project archetype aimed to create boilerplate code for a 
single-module Maven project.

## Deployment and project creation

### Local system deployment

Archetype can be deployed in a local Maven repository with

```
mvn install
```

### Creating project based on archetype

In order to create a new project the next command should be issued:

```
mvn archetype:generate                                  \
  -DarchetypeGroupId=ru.terekhov                        \
  -DarchetypeArtifactId=java-project-template           \
  -DarchetypeVersion=LATEST                             \
  -DgroupId=<my.group.id>                               \
  -DartifactId=<my-artifactId>
```

where `my.group.id` is a groupId of a newly created project, and `my-artifactId` is
its artifactId. 