[![Build Status](https://travis-ci.com/dmandalidis/lettuce-core-osgi.svg)](https://travis-ci.com/dmandalidis/lettuce-core-osgi)
[![Maven Central](https://img.shields.io/maven-central/v/org.mandas/lettuce-core-osgi.svg)](https://search.maven.org/#search%7Cga%7C1%7Cg%3A%22org.mandas%22%20lettuce-core-osgi)

This project is a fork of [Lettuce](https://github.com/lettuce-io/lettuce-core) adding only OSGi information in the
generated `MANIFEST.MF`. Its codebase is supposed to be totally aligned with the upstream repository and it is solely intended
to be used as a drop-in replacement only when OSGi bundle deployment cannot be avoided. For any other cases, please
consider using the upstream project instead. Same applies to issue handling where only OSGi-related issues will be addressed
by this project.

Not all upstream releases are enhanced by default. If you need a specific release to be enhanced, please open an issue.

Finally, branches of this project are **rebased** over the respective branches of the upstream project. This creates
a more clean git history, leaving only the fork commits at the top of the history (but ruins any attempt to clone it)

```xml
<dependency>
  <groupId>org.mandas</groupId>
  <artifactId>lettuce-core-osgi</artifactId>
  <version>x.y.z</version>
</dependency>
```