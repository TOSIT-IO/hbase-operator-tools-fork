# TDP HBase Operator tools Notes

The version 2.1.10-TDP-0.1.0-SNAPSHOT of HBase is based on the tag `rel/1.1.0` of the Apache [repository](https://github.com/apache/hbase-operator-tools/tree/rel/1.1.0).

## Making a release

```
mvn clean package -Dhadoop.profile=3.0
```

The command generates a `.jar` file of the release at `./hbase-hbck2/target/hbase-hbck2-1.1.0-0.0.jar`. 

## Testing parameters

```
mvn test -Dhadoop.profile=3.0
```

- -Dhadoop.profile=3.0: Builds with Hadoop 3 (Hadoop TDP version is set with `hadoop-three.version`)

## Test execution notes

All tests passing
