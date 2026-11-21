# WatchWolf - Tester [![CodeFactor](https://www.codefactor.io/repository/github/rogermiranda1000/watchwolf-tester/badge/dev)](https://www.codefactor.io/repository/github/rogermiranda1000/watchwolf-tester/overview/dev)
Responsable to send the commands to the rest of the WatchWolf system to test the desired plugin(s). For more information about WatchWolf check the [WatchWolf website](https://watchwolf.dev/).

The Tester is responsable of implementing WatchWolf Test's protocols. This concrete implementation will be developed using Java.

## Compile

Use a JDK supported by Gradle 9 (Java 17 or newer). The compiled Tester artifact targets
**Java 8**:

```bash
bash ./gradlew assemble
```

On Windows, use `gradlew.bat assemble`. The artifact is written to `build/libs/`.

## Release

The Gradle project version is `0.4.2`. Publish a matching GitHub Release such as `v0.4.2`
through the UI to build `watchwolf-tester-0.4.2.jar` and attach it with a SHA-256 checksum.
Tests remain disabled during normal builds because they exercise a live WatchWolf setup. Run
them explicitly with `bash ./gradlew test -PrunTests=true` against a configured environment.

### Dependencies
- `org.junit.jupiter:junit-jupiter-engine:5.8.1`
- `org.junit.jupiter:junit-jupiter-params:5.8.1`
- `org.yaml:snakeyaml:1.21`
