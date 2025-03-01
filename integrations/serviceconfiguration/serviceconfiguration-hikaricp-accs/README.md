# Service Configuration for HikariCP on Application Container Cloud Service

NOTE: This project is deprecated and slated for removal.

This project implements a Helidon Service Configuration Framework
`ServiceConfiguration` that exposes configuration information suitable
for the [Hikari connection pool](http://brettwooldridge.github.io/HikariCP/)
 when the system in effect is [Oracle's Application Container Cloud Service](https://cloud.oracle.com/acc).

## Usage

Ensure that both of the following artifacts are present on your runtime classpath:
. `serviceconfiguration-hikaricp-accs`
. `serviceconfiguration-system-oracle-accs`

When your program is running on the Application Container Cloud
Service platform, Hikari connection pool information will be made
available to programs using the Helidon Service Configuration
Framework.

## Using Oracle DB

The JDBC driver for the Oracle DB is only available from the
 [Oracle Maven Repository](https://www.oracle.com/webfolder/application/maven/index.html).

This means that you have to configure the repository in order to add the driver
 to your classpath.

Follow these steps:

- Go to https://www.oracle.com/webfolder/application/maven/index.html and
 accept the license
- Create an OTN account
- Update your settings.xml as documented [here](https://docs.oracle.com/middleware/1213/core/MAVEN/config_maven_repo.htm#MAVEN9016)
