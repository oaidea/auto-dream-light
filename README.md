# Auto Dream Light

A lightweight Auto Dream skill for OpenClaw that **adapts to an existing memory system** instead of replacing it.

---

## 中文说明

`Auto Dream Light` 是一个轻量、保守的记忆整理 skill，适合已经有自己 `MEMORY.md` / `memory/` 结构的 OpenClaw 实例。

它的目标不是接管原有记忆系统，而是：

- 扫描最近 daily log
- 提取真正值得长期保留的内容
- 增量更新现有记忆
- 记录每次 dream 的轨迹
- 支持从手动版平滑过渡到半自动版，未来再考虑 cron

它默认避免：
- 强制重建记忆架构
- 引入复杂 index / dashboard / archive
- 大规模重写 `MEMORY.md`
- 为了“显得有产出”而乱写内容

典型触发词：
- `整理记忆`
- `dream now`
- `跑 dream`
- `做一次记忆整理`
- `跑一次适配版 auto dream`

特殊查看词：
- `dream details` → 只查看最近 dream 记录，不执行新的整理

---

## English

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
