# command-mode-quickstart

## building quarkus-run

`quarkus build`

## package with jreleaser

`./mvnw -Passemble package`


## test the script
`./target/jreleaser/assemble/jrc/jlink/work-osx-aarch_64/jrc-1.0.0-SNAPSHOT-osx-aarch_64/bin/jrc `

This should run, but instead gives the following:

```
Error: Could not find or load main class io.quarkus.bootstrap.runner.QuarkusEntryPoint
Caused by: java.lang.ClassNotFoundException: io.quarkus.bootstrap.runner.QuarkusEntryPoint
```


## run the jar (without the script)
`./target/jreleaser/assemble/jrc/jlink/work-osx-aarch_64/jrc-1.0.0-SNAPSHOT-osx-aarch_64/bin/java -jar ./target/jreleaser/assemble/jrc/jlink/work-osx-aarch_64/jrc-1.0.0-SNAPSHOT-osx-aarch_64/quarkus-run.jar `

This works
