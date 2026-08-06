# Software & License Management

## Overview

End-to-end management of business software licenses and full migration of legacy applications across major version jumps, including operating system upgrades, runtime environment rebuilds, and resolution of backward-compatibility issues at the bytecode and classloader level.

## Technologies & tools

- **Trados License Manager**, **ABBYY**, **Biostar**, **TimeWalker** — business application licensing
- **Apache Tomcat** (6 → 9) — Java servlet container, legacy and current
- **Ubuntu** (10.04 → 24.04) — host OS for legacy Java applications
- **MySQL** with JDBC driver — database backend for migrated applications
- WAR / JAR analysis, classloader behavior inspection

## Responsibilities & operational scope

- Full migration of business software licenses across vendor changes (Trados License Manager, ABBYY, Biostar, TimeWalker)
- Full legacy system migration for vulnerability-assessment and remediation purposes, including:
  - OS upgrade from Ubuntu 10.04 to 24.04
  - Tomcat 6 to Tomcat 9 environment rebuild
  - Classloader and driver compatibility fixes
  - WAR reconstruction from extracted components
  - Application recovery and service restoration
  - Zero-downtime risk analysis
  - MySQL JDBC driver upgrade and refactoring of configuration paths

## Projects & evidence

### Project: Legacy Java web application migration (Ubuntu 10.04/Tomcat 6 → Ubuntu 20.04/Tomcat 9)

Executed a complex migration of a legacy Java web application from Ubuntu 10.04 with Tomcat 6 to Ubuntu 20.04 with Tomcat 9, reconstructing the entire application environment after fully recovering and analyzing configurations, JAR files, WAR structure, and classloader behavior.

Identified and resolved the failure of the JDBC pool initialization through bytecode reverse-engineering, classpath inspection, replacement of the legacy MySQL driver with a compatible version, and alignment of the properties files. Restored the correct deployment using an external `Context`, removed phantom deployments, verified binary consistency of the JARs, rebuilt the complete WAR, and enforced proper `WebappClassLoader` creation in Tomcat 9.

Ensured the stable startup of the application with the JDBC driver correctly loaded, valid configuration, and a fully functional database connection.

*Technology stack: Ubuntu 20.04, Apache Tomcat 9, MySQL JDBC, Java WAR/JAR toolchain.*

### Intel HD Graphics 4600 driver details: version 20.19.15.4531 dated 2016-09-29 (legacy)
<!-- graphify-evidence-id: 70d9301827bb -->

- **Source**: `screenshot_03.png`
- **Graph community**: 7

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

### Licensing e servizi UTM/Gold su USG FLEX 500
<!-- graphify-evidence-id: 881ad235ea3a -->

- **Source**: `shared`

*Evidence text to be enriched from source document.*

*Technology stack: to be enriched from source document.*

