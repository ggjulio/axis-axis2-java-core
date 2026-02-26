# Dependencies Behind on Latest Major Version

Dependencies in the root `pom.xml` that are not on the latest major version, based on Maven Central data.

## Successor Artifacts (Different Coordinates)

Upgrading these requires changing `groupId`/`artifactId`, not just the version number.

| Dependency | Current | Latest Major | Notes |
|---|---|---|---|
| `antlr:antlr` | 2.7.7 | 4.x | Successor is `org.antlr:antlr4-runtime` |
| `xml-resolver:xml-resolver` | 1.2 | 6.x | Successor is `org.xmlresolver:xmlresolver` |
| `bsf:bsf` | 2.4.0 | 3.1 | Successor is `org.apache.bsf:bsf-api` |

## Pre-release Only (No GA Available)

The latest major versions are not yet GA — staying on the current major is correct for now.

| Dependency | Current | Latest Major | Notes |
|---|---|---|---|
| `org.apache.maven:maven-core` | 3.9.12 | 4.0.0-rc-5 | Maven 4 is in late RC |
| `org.apache.maven.plugin-tools:maven-plugin-annotations` | 3.15.2 | 4.0.0-beta-2 | Part of the Maven 4 ecosystem |
| `org.apache.logging.log4j:log4j-bom` | 2.25.3 | 3.0.0-beta3 | Log4j 3 is still in beta |
| `org.assertj:assertj-core` | 3.27.7 | 4.0.0-M1 | AssertJ 4 is still a milestone |

## Already Addressed

| Dependency | Current | Latest Major | Notes |
|---|---|---|---|
| `junit:junit` | 4.13.2 | 5.x | `junit-jupiter` 6.0.3 is already present; JUnit 4 kept for legacy tests |

## Summary

No dependency is behind on a **GA** major version under the same coordinates. The gaps are either successor artifacts requiring migration or pre-release major versions not yet stable enough to adopt.

