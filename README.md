# JDK Serial Filter Trace

A JBoss Byteman rule to debug the trace the JDK deserialization filtering

## Foreword

Java 17 introduced Flight Recorder events for deserialization which provides a native way to figure out which classes are being serialized or deserialized using only tools included in the JDK. For more details, you can read this [article](https://inside.java/2021/03/02/monitoring-deserialization-activity-in-the-jdk/).

## TLDR

```shell
java -javaagent:/path/to/byteman.jar=script:/path/to/rules.btm,boot:/path/to/byteman.jar ...
```

Prints each call to java.io.ObjectInputStream.filterCheck() to stdout.

## Byteman

To download Byteman and to learn more about its options, see the [documentation](https://byteman.jboss.org/).

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests.

## Security

Please read [SECURITY.md](SECURITY.md) for details on our security policy and how to report security vulnerabilities.

## Code of Conduct

Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details on our code of conduct.

## License

This project is licensed under the terms of the [LICENSE](LICENSE) file.
