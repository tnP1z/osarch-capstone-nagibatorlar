# osarch-capstone-nagibatorlar

Capstone project for **IFT 103 Operating System Architecture** (Innotech University, Almaty, Fall 2026).

## What this is

A fifteen-person Almaty startup has outgrown "whoever is free sets up the laptop".
This repository contains their standard environment, built as a virtual laboratory:

- a multi-machine environment (at least one Windows node and one Linux node) and the network between them — see [`docs/architecture.md`](docs/architecture.md);
- the company hardware standard — see [`docs/hardware-standard.md`](docs/hardware-standard.md);
- automation scripts for user onboarding, inventory collection and one recurring maintenance task — see [`scripts/`](scripts/);
- runbooks for the three most likely failures — see [`runbooks/`](runbooks/);
- every significant decision with its options and cost — see [`docs/decisions.md`](docs/decisions.md).

## How to deploy it

_To be written once the environment boots end to end (milestone: week 12)._

1. Requirements on the host machine: …
2. Create the VMs: …
3. Configure the network: …
4. Run the scripts: …

A full walkthrough with evidence lives in [`evidence/deployment-walkthrough.md`](evidence/deployment-walkthrough.md).

## Team and roles

Roles agreed on: _24.11.2026_. Every member must be able to explain **every** part of the project at the defence, not only their own.

| Member | GitHub | Primary responsibility | Secondary (reviews) |
|---|---|---|---|
| Kadirzhan | @tnP1z | Infrastructure: VMs, hypervisor, network; `docs/architecture.md`, `evidence/deployment-walkthrough.md`; runbook for network/VM failure | Reviews Tolganay's Windows work |
| Marzhan Amantay | @marzhanNagibator777 | Linux node; bash scripts (inventory collection, scheduled maintenance); `scripts/bash/README.md`; runbook for a Linux failure | Reviews Kadirzhan's infrastructure |
| Tolganay Nursapa | @Tolganayy0806 | Windows node; PowerShell onboarding script; `docs/hardware-standard.md`; runbook for a Windows failure | Reviews Marzhan's Linux work |

## Who did what

The detailed week-by-week record is in [`docs/build-log.md`](docs/build-log.md). The commit history is the evidence.

## Working rules

- Everyone commits from their **own** GitHub account (teamwork is graded on commit history).
- Folder and file names: Latin letters, lower case, hyphens instead of spaces.
- Command output goes into `.txt` files; screenshots (`.png`) only when the thing shown is genuinely visual.
- Every decision that someone could ask "why?" about goes into `docs/decisions.md` the same day.
- Bash scripts must pass ShellCheck with no warnings.

## Milestones

| Week | What should exist | Status |
|---|---|---|
| 9 | Team formed, repository created, roles agreed in this README | in progress |
| 10 | `architecture.md` drafted | |
| 12 | Environment boots end to end | |
| 13 | First script working, `hardware-standard.md` drafted | |
| 14 | Both shells represented, runbooks drafted | |
| 15 | Another team tests our runbooks; fixes made | |
| 16 | Demonstration and defence | |
