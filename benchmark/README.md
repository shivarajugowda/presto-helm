# Run benchmarks

## Download jar files

```
curl https://repo1.maven.org/maven2/io/prestosql/presto-cli/334/presto-cli-334-executable.jar -o presto-cli-334-executable.jar
```

```
curl https://repo1.maven.org/maven2/io/prestosql/presto-benchto-benchmarks/334/presto-benchto-benchmarks-334-executable.jar -o presto-benchto-benchmarks-334-executable.jar
```


```
java -Xmx1g -jar presto-benchto-benchmarks-*-executable.jar \                                                           
    --sql resources/sql \
    --benchmarks resources/benchmarks \
    --activeBenchmarks=presto/tpch --profile=presto-devenv \
    --overrides overrides.yaml
```
