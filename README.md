# WatchWolf - Tester [![CodeFactor](https://www.codefactor.io/repository/github/rogermiranda1000/watchwolf-tester/badge/dev)](https://www.codefactor.io/repository/github/rogermiranda1000/watchwolf-tester/overview/dev)
Responsable to send the commands to the rest of the WatchWolf system to test the desired plugin(s). For more information about WatchWolf check the [WatchWolf website](https://watchwolf.dev/).

The Tester is responsable of implementing WatchWolf Test's protocols. This concrete implementation will be developed using Java.

## Compile
Use Java **8**.

## Release

The Maven project version is `0.4.0`. Push a matching tag such as `v0.4.0` to build
`watchwolf-tester-0.4.0.jar` and publish it with a SHA-256 checksum in a GitHub Release.
The release build uses the POM's existing test skip setting; run the integration tests
against a live WatchWolf setup separately.

### Dependencies
- Maven's `org.junit.jupiter:junit-jupiter-engine:5.8.1`
- Maven's `org.junit.jupiter:junit-jupiter-params:5.8.1`
- Maven's `org.yaml:snakeyaml:1.21`
