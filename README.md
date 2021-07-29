# jdk-serial-filter-trace

A JBoss Byteman rule to debug the trace the JDK deserialization filtering

## TLDR

```
java -javaagent:/path/to/byteman.jar=script:/path/to/rules.btm,boot:/path/to/byteman.jar ...
```

Prints each call to java.io.ObjectInputStream.filterCheck() to stdout.

## Byteman

To download Byteman and to learn more about its options, see https://byteman.jboss.org/.
