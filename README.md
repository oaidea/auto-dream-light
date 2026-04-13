# Auto Dream First

A lightweight Auto Dream skill for OpenClaw that **adapts to an existing memory system** instead of replacing it.

## Positioning

Most Auto Dream-style memory systems assume they can reshape your whole memory architecture.
This skill takes the opposite approach:

- preserve the current `MEMORY.md` structure
- preserve existing project memory files
- consolidate only what is durable and high-value
- keep execution conservative and easy to audit

## What it does

- scans recent daily logs
- extracts decisions, durable facts, stable preferences, project milestones, reusable lessons
- routes memory to the right destination
- updates memory incrementally
- records each run in a lightweight dream log
- supports a gradual path from manual → semi-automatic → cron later

## What it avoids

- no forced new memory architecture
- no dashboards by default
- no index.json by default
- no archive system by default
- no aggressive rewrites of `MEMORY.md`
- no fake output when there is nothing worth saving

## Included references

- `references/adapted-plan.md`
- `references/manual-run.md`
- `references/semi-auto.md`

These define:
- design principles
- manual execution flow
- semi-automatic trigger-based flow

## Recommended usage

Start with manual runs.
Only move toward semi-automatic or cron-based execution after several stable runs.

## Trigger phrases

Typical triggers:
- `整理记忆`
- `dream now`
- `跑 dream`
- `做一次记忆整理`
- `跑一次适配版 auto dream`

Special viewer trigger:
- `dream details` → show recent dream history without starting a new run
