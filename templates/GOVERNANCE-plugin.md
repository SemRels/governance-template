# Governance

## Overview

This SemRels plugin repository is governed by its maintainers and community contributors. Plugin repositories focus on plugin APIs, plugin implementations, and release compatibility with the SemRels core toolchain.

## Scope

This governance applies to plugin code, examples, release automation, and supporting documentation in the repository.

## Decision Making

Routine plugin changes use lazy consensus. Changes that affect compatibility, plugin APIs, or release behavior should be proposed in an Issue before merge.

## Maintainer Expectations

- At least one maintainer approval is required for pull requests.
- Compatibility-impacting changes should be reviewed by a maintainer responsible for plugin architecture.
- Release process changes should be documented in the repository before adoption.
- Every plugin must implement the SemRels dry-run contract (`SEMREL_DRY_RUN=true`): emit `plugin_schema_version=1` and human-readable log lines on `stderr`, emit unified diffs/content blocks/commands/payloads on `stdout`, fail soft when publishing credentials are absent, and perform zero side effects.
