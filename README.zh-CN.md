# Auto Dream Light

一个适用于 OpenClaw 的轻量 Auto Dream 技能。

`Auto Dream Light` 面向已经拥有自己 `MEMORY.md` 与 `memory/` 工作流的 OpenClaw 实例。

它的目标不是接管你现有的记忆系统，而是帮助 agent：

- 扫描最近的 daily log
- 提取真正值得长期保留的信息
- 按现有结构增量更新记忆
- 为每次整理留下轻量 dream-log
- 从手动版平滑过渡到半自动版，未来再考虑 cron

## 为什么做这个 skill

很多记忆类方案喜欢一上来就重建整套架构。

`Auto Dream Light` 反过来：
- 保留原有结构
- 保守写入
- 跳过噪音
- 不伪造“产出感”
- 保持可审计、可回看

## 它会做什么

- 扫描最近的 daily log
- 抽取决策、长期事实、稳定偏好、项目里程碑、可复用经验
- 将信息路由到正确的目标位置
- 以增量方式更新记忆
- 为每次运行写入轻量 dream-log
- 支持从手动版逐步走向半自动版，未来再接 cron

## 它默认不会做什么

- 不强制重建记忆架构
- 不默认引入 dashboard
- 不默认引入 index.json
- 不默认引入 archive 系统
- 不大规模重写 `MEMORY.md`
- 没有值得沉淀的新内容时，不会硬写

## 仓库内包含的参考文件

- `references/adapted-plan.md`
- `references/manual-run.md`
- `references/semi-auto.md`

分别对应：
- 设计原则
- 手动执行流程
- 半自动触发式流程

## 推荐使用方式

先从手动执行开始。
等多次运行稳定后，再考虑进入半自动版或 cron 自动化。

## 典型触发词

- `整理记忆`
- `dream now`
- `跑 dream`
- `做一次记忆整理`
- `跑一次适配版 auto dream`

特殊查看词：
- `dream details` → 只看最近 dream 记录，不触发新的整理
