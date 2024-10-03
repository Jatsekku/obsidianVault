## Quick intro
- platform for automating works execution (workflows) triggered by specified events
- may serve as CI/CD system
- fully integrated with [github](https://github.com/)

## Key functionalities
- Can run on Linux, macOS, Windows and containers
- Logging mechanism (realtime, search engine, creating links to specific logs)
- Secret store
- Matrix build (idk what that means yet)

## Overview
based on: [Understanding GitHub Actions](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions)
### Steps
- Step is smallest execution unit in Github Actions
- It can run script, command, set of commands or [[#actions|action]]
- Set of steps creates [[#jobs|job]]
- Steps in same [[#jobs|job]] are executed sequentially, on the same runner
- Steps in same [[#jobs|job]] can share data

### Actions
- it's custom application from Github Actions platform
- Manages typical tasks associated with repo management (i.e. pull, checkout, etc)

### Jobs
- Job is set of [[#steps]]
- By default, jobs run in parallel and have no dependencies
- Job can be configured to be dependent on another job - in that case it waits with execution until dependent job is finished.

### Workflow
- Consist one or more [[#Jobs|jobs]]
- Triggered by [[#Events (triggers)|event]]

### Runners
- Server executing worflows
- Run single [[#Jobs|job]] at a time
- Can use GitHub provided runners or self-hosted ones

### Events (triggers)
[[#Workflow]] can be triggered:
- by repository event (i.e. push, pull request, new issue etc)
- by posting to REST API
- on defined schedule
- manually

![[GithubActions_overview.png]]

## Running workflows locally

## Materials
- [# How to test GitHub Actions Locally!!!](https://www.youtube.com/watch?v=YORvmxQBPeM&ab_channel=IsaacLevin) - YT video going through act functionalities and usage
