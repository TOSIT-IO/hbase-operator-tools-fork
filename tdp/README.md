# TDP HBase Operator tools Notes

The version 1.2.0-0.0 of HBase Operator Tools is based on the tag `rel/1.2.0` of the Apache [repository](https://github.com/apache/hbase-operator-tools/tree/1.2.0RC1).

## Making a release

```
mvn clean install -Dhadoop.profile=3.0 -DskipTests
```

The command generates a `.jar` file of the release at `./hbase-hbck2/target/hbase-hbck2-1.2.0-0.0.jar`.

## Testing parameters

```
mvn test -Dhadoop.profile=3.0
```

- -Dhadoop.profile=3.0: Builds with Hadoop 3 (Hadoop TDP version is set with `hadoop-three.version`)

## Test execution notes

All tests passing
