# 案例：microsoft/playwright-mcp

## 项目类型
工具型项目。

## 快速判断
这是一个**定位清楚、范围集中、容易做精确判断**的工具项目。

## 为什么值得看
- 价值主张清晰：给 MCP 客户端提供 Playwright 浏览器自动化
- README 对 MCP vs CLI 的边界解释得比较清楚
- 仓库范围相对集中，容易对照 README 与代码结构

## 风险点
- 作为工具项目，真正的问题会集中在边界条件和兼容性
- issue 列表里常见的是特殊字符、扩展 attach、context 等细节问题
- 对 agent 来说，还要额外考虑 token / context 成本

## 评分示例
- Practical utility: 4
- Local fit: 3
- Operational burden: 4
- Reliability: 4
- Adoption worthiness: 4
- Total: 19/25

## adopt / adapt / avoid
- **Adopt directly**：适合明确需要 MCP 浏览器控制的环境
- **Adapt**：如果本地已有更贴近场景的浏览器 skill，不必机械引入
- **Avoid blindly**：不要把“微软出品 + README 清楚”直接等同于所有边界情况都稳

## 学到的规则
工具型项目更适合：
- 对核心循环做精确判断
- 对边界 bug 做现实预估
- 对 token/context 成本做额外评估
