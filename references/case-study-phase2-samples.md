# 第二阶段样本：项目类型对判断方法的影响

这轮实战选了 3 个不同类型的 GitHub 项目：

1. `openclaw/openclaw` — 平台型项目
2. `microsoft/playwright-mcp` — 工具型项目
3. `OpenHands/OpenHands` — 平台型项目

## 这轮学到的关键点

### 1. 不能用同一把尺子看所有项目
- 平台型项目：范围大、issue 多、PR 多，本身不代表不稳定
- 工具型项目：范围更窄，README 承诺更容易和实现逐项对照
- scaffold/aggregator 型项目：要重点看“路由价值”和“维护代价”的平衡

### 2. README 很强，不代表落地成本低
从这轮样本里再次确认：
- 强 README 能证明定位清晰
- 不能证明低维护、低复杂度、低摩擦
- 越是看起来“全能”的项目，越要防止被叙事带着走

### 3. 平台型项目更要看维护能量，而不是只看 open issues 数
像 OpenClaw、OpenHands 这类仓库：
- open issues 多是正常现象
- 更重要的是提交/PR/文档/更新是否持续活跃
- 要看它是不是在持续处理复杂系统的真实问题

### 4. 工具型项目更适合做精确判断
像 `microsoft/playwright-mcp` 这种：
- 价值主张更窄
- 更容易判断核心循环是否可靠
- 更容易发现边界问题是不是会伤到主要用途

## 反哺到 skill 的改进
因此新增两类长期规则：

- `project-types.md`
  - 平台 / 工具 / scaffold 分型判断
- `readme-vs-reality.md`
  - 用于识别 README 叙事和真实实现之间的差距
