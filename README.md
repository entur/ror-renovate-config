# ror-renovate-config

Common renovate bot config for RoR projects.

Default base branch is `master`, override if necessary.

Use by extending in your local renovate.json:

```
{
  "extends": [
    "github>entur/ror-renovate-config",
  ]
}
```

## Group non-major upgrades

An additional preset is available which will group non-major upgrades in a weekly pull request:

```
{
  "extends": [
    "github>entur/ror-renovate-config",
    "github>entur/ror-renovate-config:groupNonMajorWeekly"
  ]
}
```

## Exceptions

 * Disabled updates for `nexus-staging-maven-plugin` due to [NEXUS-26993](https://issues.sonatype.org/browse/NEXUS-26993)