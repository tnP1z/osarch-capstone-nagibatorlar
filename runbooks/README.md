# Runbooks

Three runbooks for the three most likely failures, named `01-<failure>.md`, `02-<failure>.md`, `03-<failure>.md`.
Written so that somebody else can follow them — another team will test them in week 15.

Template for each runbook:

```
# <Failure name>

**Symptom:** what the user reports / what you see.
**Affected:** which nodes, which users.
**Before you start:** access and tools you need.

## Diagnose
1. Command → expected output → what it means.

## Fix
1. …

## Verify
1. …

## If this did not work
Escalate to … / try …
```
