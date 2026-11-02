# Unified Reading Implementation Plan

> **For agentic workers:** Use executing-plans to implement this plan task-by-task. User approved the design and implementation in this conversation.

**Goal:** 统一阅读并增强方法讲解，保留审稿、对比及证据边界。
**Architecture:** 入口负责路由；阅读模板负责叙事；讲解和可视化参考按需加载。
**Tech Stack:** Markdown；验证工具不构成技能运行依赖。
**Spec:** [已确认设计](../specs/2026-11-02-unified-reading-design.md)

## Global Constraints

无固定阅读子模式；用户深度、顺序与格式优先；无新增运行时依赖；不发布。

## Review Focus

- 审稿视角讲解不变成审稿报告。
- 逐章请求保持编号及覆盖，局部问题不重启全篇。
- 摘要不足以补全方法或复现情况。
- 示例、曲线不冒充实验结果。
- 理论论文不套用训练检查表，不匹配的实验不排名。

## Tasks

- [x] 1. 保存合成输入与请求，运行旧技能基线；记录实际行为。
- [x] 2. 重写入口和阅读指导，新增讲解与可视化参考，清理旧指引；同步 README 和忽略规则。
- [x] 3. 用新技能执行场景，审查实际输出；检查 frontmatter、链接、旧类型残留及 diff；保存验证范围和结果。

## Execution notes

在当前已授权工作区修改文档，不创建环境或运行应用。基线与新版行为使用独立上下文验证，未发生的失败不追认；合成测试不代表真实 PDF 或渲染集成验证。

验证环境例外：为运行官方 frontmatter 检查，在临时目录用 uv 创建 Python 3.12.10 环境并通过 uv add 安装 PyYAML；未加入技能依赖。基线没有观察到模式误判，保留原始输出。变更基于已确认的新设计，不伪造失败先例。

执行完成：新版 10 个场景输出已经人工核对，R7 仅验证 SVG 结构和数学内容，未验证渲染；独立文档一致性审查无可行动问题。完整范围与限制见 [验证记录](../../../tests/validation-2026-11-02.md)。未自动提交、安装或发布。
