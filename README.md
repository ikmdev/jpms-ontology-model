# jpms-ontology-model
The jpms-ontology-model repository is dedicated to making the ontology-model module compliant with the Java Platform Module System (JPMS). This compliance ensures that the ontology-model library can be seamlessly integrated into modular Java applications, leveraging the benefits of JPMS such as improved encapsulation, security, and maintainability.

## Features

* **JPMS Compliance:** The library is packaged as a JPMS module, enabling better encapsulation and dependency management in Java projects.
* **Ease of Use:** Simple integration into projects using JPMS.

## Getting Started
### Prerequisites

* **Java 11 or higher:** JPMS was introduced in Java 9, so a minimum of Java 11 is recommended for compatibility and support.
* **Maven or Gradle:** For dependency management and building the project.

Add the following dependency to your pom.xml:
```xml
<dependency>
    <groupId>dev.ikm.jpms</groupId>
	<artifactId>ontology-model</artifactId>
    <version>${latest-jpms-ontology-model-version}</version>
</dependency>
```

Add the following dependency to your build.gradle:
```groovy
implementation 'dev.ikm.jpms:ontology-model:${latest-jpms-ontology-model-version}'
```

In your module descriptor (module-info.java), declare the dependency on the jpms-ontology-model module:

```java
module your.module.name {
    requires dev.ikm.jpms.hl7.tinkar.snorocket;
}
```


## Issues and Contributions
Technical and non-technical issues can be reported to the [Issue Tracker](https://github.com/ikmdev/jpms-ontology-model/issues).

Contributions can be submitted via pull requests. Please check the [contribution guide](doc/how-to-contribute.md) for more details.