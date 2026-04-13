---
name: auto-dream-light
version: 0.1.0
description: Lightweight, memory-safe Auto Dream workflow for OpenClaw that adapts to an existing memory system instead of replacing it. Use when users want periodic or on-demand memory consolidation, dream logs, or a gradual path from manual memory cleanup to semi-automatic consolidation without forcing a new memory architecture.
---

# Auto Dream Light

A conservative Auto Dream skill for OpenClaw instances that already have their own memory structure.

## What this skill is for

Use this skill when the user wants:
- on-demand memory consolidation
- a lightweight “dream” workflow
- a dream log with execution history
- a gradual upgrade path from manual to semi-automatic memory cleanup
- memory consolidation **without** replacing the current `MEMORY.md` structure

This skill is intentionally conservative:
- it does **not** rebuild the memory architecture
- it does **not** introduce dashboards, indexes, or archives by default
- it does **not** assume the user's memory follows a template
- it prefers small, explicit, high-value updates

## Core idea

Instead of forcing a new memory system, this skill works with the one the user already has.

Default approach:
1. scan recent daily logs
2. extract durable, high-value information
3. route items to the correct destination
4. update memory incrementally
5. record the run in a dream log
6. return a concise summary to the user

## Read these references when needed

- Read `references/adapted-plan.md` before designing or changing the workflow.
- Read `references/manual-run.md` when running the workflow manually.
- Read `references/semi-auto.md` when the user wants a fixed trigger-based flow or wants to prepare for cron later.

## Default file roles

Typical targets:
- `MEMORY.md` → long-term facts, stable preferences, system conclusions, reusable lessons
- `memory/projects/**` → project-specific context
- `memory/system/auto-dream-log.md` → dream execution history only
- `memory/YYYY-MM-DD.md` → raw daily notes; only add a consolidation marker when appropriate

## Operating rules

- Preserve the existing memory structure.
- Prefer project files over stuffing everything into `MEMORY.md`.
- Skip low-value chat, tests, and one-off noise.
- Do not invent memory just to make a run look productive.
- If there is nothing worth consolidating, explicitly skip and say so.

## Trigger guidance

Typical trigger phrases:
- "整理记忆"
- "dream now"
- "跑 dream"
- "做一次记忆整理"
- "跑一次适配版 auto dream"

If the user says `dream details`, show recent dream-log history instead of running a new consolidation.
