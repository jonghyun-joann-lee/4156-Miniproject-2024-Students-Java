# Static Bug Finder

To check for bugs, I used **PMD** as the static bug finder. I used the error-prone and default rulesets, which were configured like below in the pom.xml file.

```
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-pmd-plugin</artifactId>
    <version>3.25.0</version>
    <configuration>
        <rulesets>
            <ruleset>/category/java/errorprone.xml</ruleset>
            <ruleset>/rulesets/java/maven-pmd-plugin-default.xml</ruleset>
        </rulesets>
    </configuration>
</plugin>
```

To run PMD, I used the following command in the terminal from the root of the Maven project.

`mvn pmd:check`