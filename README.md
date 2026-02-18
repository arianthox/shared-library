# shared-library

## Overview

Jenkins shared library for reusable CI pipeline helpers used by BrainWaves repositories.

## Scope in BrainWaves

- CI/CD support only (not runtime application logic)
- Shared step currently includes Slack notifications

## Tech Stack

- Groovy
- Jenkins Shared Library conventions

## Build

- N/A (interpreted by Jenkins)

## Run

- Used from Jenkins pipelines

## Key Configuration / Integration

- Main shared step:
  - `vars/slackNotificator.groovy`
- Imported by Jenkinsfiles as:

```groovy
@Library('jenkins-shared-library')_
```

## Status / Notes

- Keep helper APIs stable to avoid breaking pipeline compatibility.
