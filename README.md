# Project Maven Archetype

This project is a custom Maven archetype for quickly bootstrapping new Spring Boot projects default conventions and structure.

---

## 🚀 Features

- Spring Boot 3.4.4
- Java 17
- Optional Spring Web, JPA, Lombok, Testcontainers support (via Velocity conditions)
- Preconfigured plugins: JaCoCo, Spotless, Swagger OpenAPI, JUnit 5, Mockito

---

## 📦 Installation

To install the archetype locally (make it available in your local Maven cache):

```bash
git clone https://github.com/gabin-ishimwe/project-archetype.git
cd project-archetype
mvn clean install -Darchetype.test.skip=true
```
---
## ⚙️ Generate Project
```bash
mvn archetype:generate \
  -DarchetypeGroupId=com.project.project \
  -DarchetypeArtifactId=project-archetype \
  -DarchetypeVersion=1.0-SNAPSHOT \
  -DgroupId=com.mycompany.app \
  -DartifactId=my-service \
  -Dversion=0.0.1-SNAPSHOT \
  -Dwith-spring-web=true \
  -Dwith-spring-jpa=true \
  -Dwith-lombok=true \
  -Dwith-testcontainers=false \
  -DinteractiveMode=false