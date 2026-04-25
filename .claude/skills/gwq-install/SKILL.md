---
name: gwq-install
description: Build and install gwq from this fork project. Use when you want to rebuild and apply the local gwq binary to replace the system gwq command.
allowed-tools: Bash
user-invocable: true
disable-model-invocation: true
---

# gwq Install

This project is a fork of gwq. Use this skill to build and install the local version, replacing the system-installed gwq binary.

## Usage

```
/gwq-install
```

## Behavior

Run the following steps:

1. Run `make install` in the project root (`/Users/takuya/workspace/github.com/AniP-gt/gwq`)
2. Confirm the installed binary path with `which gwq`
3. Confirm the version with `gwq version`
4. Report the result to the user

## Steps

```bash
cd /Users/takuya/workspace/github.com/AniP-gt/gwq && make install
which gwq
gwq version
```

If `make install` fails, show the error output and stop.
