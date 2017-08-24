## Overview
This is a simple set up for test driving PySpark scripts. It is fairly portable, as all you need to use it are:
- `docker` version 17.06.1-ce or greater
- `docker-compose` version 1.14.0 or greater
- PyCharm Ultimate edition 2017.2 or greater (need ultimate for Docker based interpreter setup)

## Using
Run tests and build the test/dependency docker
```sh
docker-compose build test
```

As you make changes, run tests via that docker
```sh
docker-compose build test
```

-or- run tests inside of the PyCharm Ultimate IDE
1. Configure PyCharm to talk to Docker
2. Configure a remote interpreter for this project and have it use `pyspark-fun-test` as the docker that provides the interpreter