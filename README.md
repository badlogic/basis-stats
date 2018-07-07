# basis-stats
Basis-stats parses web server log files and transforms them into statistics such as unique visitors, bandwidth, etc. All statistics are kept in memory and can optionally be updated live from changes to the input log file.

## Motivation
Why another argument log analyzer library?

* Does not depend on a specific web server.
* Provides live statistics by observing changes to the log file.
* Zero dependencies.

## Setup
As a dependency of your Maven project:

```
<dependency>
   <groupId>io.marioslab.basis</groupId>
   <artifactId>stats</artifactId>
   <version>1.0</version>
</dependency>
```

As a dependency of your Gradle project:
```
compile 'io.marioslab.basis:stats:1.0'
```

You can also build the `.jar` file yourself, assuming you have Maven and JDK 1.8+ installed:
```
mvn clean install
```

The resulting `.jar` file will be located in the `target/` folder.

You can also find `SNAPSHOT` builds of the latest and greatest changes to the master branch in the SonaType snapshots repository. The snapshot is build by [Jenkins](https://libgdx.badlogicgames.com/jenkins/job/basis-stats/)

To add that snapshot repository to your Maven `pom.xml` use the following snippet:

```
<repositories>
    <repository>
        <id>oss-sonatype</id>
        <name>oss-sonatype</name>
        <url>https://oss.sonatype.org/content/repositories/snapshots/</url>
        <snapshots>
            <enabled>true</enabled>
        </snapshots>
    </repository>
</repositories>
```

Google will tell you how to do the same for your Gradle builds.

## Basic Usage

## License
See [LICENSE](./LICENSE)

## Contributing
Simply send a PR and grant written, irrevocable permission in your PR description to publish your code under this repository's [LICENSE](./LICENSE).
