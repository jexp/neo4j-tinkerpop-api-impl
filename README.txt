Implementation of Apache Licensed Neo4j API for Tinkerpop3
==========================================================

This repository contains the implementation of the `neo4j-tinkerpop-api` as `neo4j-tinkerpop-api-impl`

This work depends on neo4j-gremlin being updated to use the latest version of `neo4j-tinkerpop-api(-impl)`.

To build:

````
# build neo4j-tinkerpop-api

git clone github.com/neo4j-contrib/neo4j-tinkerpop-api
cd neo4j-tinkerpop-api
mvn clean install
cd ..

# build neo4j-tinkerpop-api-impl

git clone github.com/neo4j-contrib/neo4j-tinkerpop-api-impl
cd neo4j-tinkerpop-api-impl
mvn clean install

# build tinkerpop3 branch with neo4j-gremlin updated

git clone https://github.com/jexp/incubator-tinkerpop
cd incubator-tinkerpop/neo4j-gremlin
mvn clean install
# skip enforcer 
# mvn clean install -DincludeNeo4j -Denforcer.skip=true
cd ..

```
Results :

Tests run: 4133, Failures: 0, Errors: 0, Skipped: 601

[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 28:18 min
```
