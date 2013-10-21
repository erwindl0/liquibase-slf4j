# liquibase-slf4j
Version 1.2.1<br/>
Written by Matt Bertolini

## How to Use
Grab the library from Maven Central and place it in your classpath.

**Maven:**

```xml
<dependency>
    <groupId>com.mattbertolini</groupId>
    <artifactId>liquibase-slf4j</artifactId>
    <version>1.2.1</version>
</dependency>
```

**Gradle:**

```groovy
runtime group: 'com.mattbertolini', name: 'liquibase-slf4j', version: '1.2.1'
```

**Ivy**

```xml
<dependency org="com.mattbertolini" name="liquibase-slf4j" rev="1.2.1"/>
```

## License
liquibase-slf4j is licensed under the [MIT License](http://www.opensource.org/licenses/mit-license.php)

## Notes
This logger has a priority number of 5. If you have more than one Liquibase logger on your classpath the one with the
highest priority will be used.

## Build and Test
### Requirements
* [Apache Ant](http://ant.apache.org/) - Version 1.8 or higher.
* JDK 6 or higher (Compiled with 1.6 source and target).

### Build
To build this project, clone the repo and run the ```ant``` command:
```
$ git clone https://github.com/mattbertolini/liquibase-slf4j.git
$ cd liquibase-slf4j
$ ant
```

The distributable jar files will be located in the ```dist``` folder. The build reports (unit test, dependency,
coverage, etc.) will be located in the ```build/reports``` dir.

To run the unit tests run the ```run-unit-tests``` task.
```
$ ant run-unit-tests
```

## Bugs
Please report any bugs in the issue tracker above. Please be as detailed as possible in your report so I can create
unit tests to verify the problem is fixed.

## Release Notes

**1.2.1 - 2013-10-12**

* Only printing the changeLogName and changeSetName if they are provided. This gets rid of the annoying nulls printed
in logs.

**1.2.0 - 2013-09-30**

* Upgrading to Liquibase version 3.0.5 to add new required methods.

**1.1.0 - 2013-08-10**

* Upgrade Liquibase version to 3.0.x.
* Backward-compatible with previous version.

**1.0.0 - 2012-04-04**

* Initial release.
* Supports Liquibase 2.0.x.
