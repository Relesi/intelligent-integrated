[![JetBrains incubator project](https://jb.gg/badges/incubator.svg)](https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub)
[![Apache license](https://img.shields.io/badge/license-Apache%20License%202.0-blue.svg?style=flat)](https://www.apache.org/licenses/LICENSE-2.0)
[![Download](https://img.shields.io/maven-central/v/org.jetbrains.kotlinx/kotlinx-knit/0.2.2)](https://search.maven.org/artifact/org.jetbrains.kotlinx/kotlinx-knit/0.2.2/pom)

[![Build Status](https://www.travis-ci.com/Relesi/inteligent-integrated.svg?branch=master)](https://www.travis-ci.com/Relesi/inteligent-integrated)
## Integrated Guide

**Using gradle?** See [gradle example](https://github.com/Relesi)

### Travis Setup

Add to your `.travis.yml` file.
```yml
language: java
after_success:
  - bash <(curl -s https://codecov.io/bash)
```
### Produce Coverage Reports
#### Add Jacoco plugin
```xml
<plugin>
  <groupId>org.jacoco</groupId>
  <artifactId>jacoco-maven-plugin</artifactId>
  <version>0.7.9</version>
  <executions>
    <execution>
      <goals>
        <goal>prepare-agent</goal>
      </goals>
    </execution>
    <execution>
      <id>report</id>
      <phase>test</phase>
      <goals>
        <goal>report</goal>
      </goals>
    </execution>
  </executions>
</plugin>
```

### Private Repos
Add to your `.travis.yml` file.
```yml


Development...


