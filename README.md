= MySQL

NOTE: This config is currently untested.

OpenNMS configuration files for collecting MySQL metrics.

== Installation

.Download and install from GitHub
[source, bash]
----
mkdir ${HOME}/opennms-config-workspace
cd ${HOME}/opennms-config-workspace
git clone https://github.com/opennms-config-modules/mysql.git
----

=== MySQL driver

Download the driver here https://mvnrepository.com/artifact/mysql/mysql-connector-java
and save the jar file into `/var/opennms/lib/`.

=== Data Collection

.Install datacollection configuration

Add the package `MySQL` into `jdbc-datacollection-config.xml` with the one provided in `datacollection/postgresql.xml`.

Add the content of `collectd-config-xml` into the existing one in your setup.
