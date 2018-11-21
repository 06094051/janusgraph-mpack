# JanusGraph Mpack

An Ambari management pack based implementation of JanusGraph.

This is heavily based on the JanusGraph Ambari service at https://github.com/chupman/janusgraph-ambari-service

## Installing

The MPack can be installed with:

```
ambari-server install-mpack --mpack URL_TO_MPACK_FILE
```

You will then be able to add the service to an HDP 2.6 cluster that has HBase and Solr running on it.

## Building

The maven pom file will build an mpack in the target direction with `mvn clean package`

Note that the mpack also depends on an available rpm repo containing the actual JanusGraph releases. Information on this can be found at https://github.com/simonellistonball/janusgraph-rpm