# TFB Databases

This project houses all the databases that can be built and published 
containers to be used on the [TechEmpower Framework Benchmarks](https://github.com/TechEmpower/FrameworkBenchmarks)
project.

## Structure

Each folder represents a single database, and each database folder houses a 
`Dockerfile` and all materials required by said `Dockerfile` for building an
image which can be run in Docker.

## Versioning

TODO - Not sure right now... `:latest` feels wrong, but how would we 
communicate versions between here and Dockerhub and then also back to the 
toolset? It may be worth tagging every build with a version, known here, and
`:latest`, that way the toolset could use `:latest` but it would also 
correspond with a known version at any moment in time.

## Publishing

When a new database has been added, or an existing database updated, a 
publish-event must occur before the [TFBToolset](https://github.com/TechEmpower/TFBToolset)
will be able to use it. 

TODO - how to publish a build given the above version rules.
  
## Authors

* **Mike Smith** - *Initial work* - [msmith](https://github.com/msmith-techempower)

## License

This project is licensed under the BSD-3-Clause License - see the [LICENSE.md](LICENSE.md) file for details

  