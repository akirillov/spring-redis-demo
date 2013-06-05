Spring Data - Redis Twitter Example for Maven
---------------------------------------------

An improved Java implementation of the [Redis Twitter Clone](http://redis.io/topics/twitter-clone) using Spring Data. Tutorial available [here](http://static.springsource.org/spring-data/data-keyvalue/examples/retwisj/current/)

Live instance available on [CloudFoundry](http://www.cloudfoundry.com/) [here](http://retwisj.cloudfoundry.com/)

### Fork Features
The main point of this fork is to exclude Gradle from build and switch to Maven.
The idea behind is that Gradle still causes some issues with IDE integration and just build a WAR is not the goal of the demo.

Overall repository structure has been changed to contain just Redis example and may be will be extended to future KV samples.

### IntelliJ IDEA
As for IDEA 11 it is necessary to configure "exploded war" artifact to run the demo.

### Build
Just run the following command in the directory You've just cloned.

    $ mvn clean package

It will compile and package all the files into resulting WAR. Start up an instance of the Redis server, deploy your WAR and point your browser to (for the typical setup) [http://localhost:8080/retwisj](http://localhost:8080/retwisj)