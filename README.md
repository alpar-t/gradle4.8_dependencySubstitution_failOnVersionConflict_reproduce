Reproduce gradle/gradle#5692 with Gradle 4.8

Run:
```
./gradlew assemble
```
It fails with:
```
* What went wrong:
Could not determine the dependencies of task ':compileJava'.
> Could not resolve all dependencies for configuration ':compileClasspath'.
   > A conflict was found between the following modules:
      - gradle_test:sub1:0.0.1
      - gradle_test:sub1:0.0.1

```
Works with Gradle 4.7
