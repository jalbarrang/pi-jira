# @dreki-gg/pi-jira

## [0.3.1](https://github.com/jalbarrang/pi-jira/compare/v0.3.0...v0.3.1) (2026-07-12)


### Bug Fixes

* **deps:** bump dependencies to latest ([#4](https://github.com/jalbarrang/pi-jira/issues/4)) ([d8d7545](https://github.com/jalbarrang/pi-jira/commit/d8d7545035e8d51c485f63345a8ee322c6e13b44))

## [0.3.0](https://github.com/jalbarrang/pi-jira/compare/v0.2.0...v0.3.0) (2026-07-11)


### Features

* extract pi-jira from dreki-gg/pi-extensions monorepo ([a0bb65c](https://github.com/jalbarrang/pi-jira/commit/a0bb65c7c2030ad5353540f3f7f733c133437165))

## 0.2.0

### Minor Changes

- New extension: Jira tools backed by an authenticated Atlassian CLI (`acli`)
  session. `jira_view` pulls a ticket's description and comments into context,
  `jira_search` runs JQL queries, `jira_comments` reads a ticket's thread, and
  `jira_comment` posts a concise comment back. Every read tool returns a compact
  digest inline and writes the full, untruncated output to a temp file (so long
  descriptions and comment threads survive harness truncation — the agent reads
  the file). A `/jira` command reports auth and config status, and `.pi/jira.json`
  supports `acliPath`, `defaultProject`, `viewFields`, and `searchLimit`.
