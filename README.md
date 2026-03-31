# Internet Reach

一个为当前 OpenClaw 工作区定制的互联网研究与项目评估技能。

## 这是什么

`internet-reach` 不是一个“大而全安装器”，而是一个**研究路由 + 实用性判断 + 学习沉淀**技能。

它的目标不是替代所有外部工具，而是帮助智能体在当前环境里更稳定地完成这些任务：

- 看 GitHub 项目、Issue、PR、提交记录
- 读网页、文档、文章、说明页
- 判断一个工具/项目到底值不值得用
- 区分“营销承诺”和“实际可落地性”
- 把外部项目的方法论吸收成当前工作区可复用的长期能力

## 适用场景

适合这些请求：

- “去 GitHub 学一下这个项目”
- “分析一下这个 repo 的实用性”
- “看看这个工具值不值得装”
- “读一下这个链接，然后提炼重点”
- “你也学一下，变成你自己的 skill”

## 当前设计原则

1. **GitHub 优先**：涉及 GitHub 就先用 GitHub 能力，而不是先搜网页。
2. **已知 URL 直读**：用户给了链接，就先直接读链接。
3. **证据优先级明确**：代码 / 文档 / issue / PR / 提交记录 > 营销文案。
4. **小而稳**：优先吸收方法，不盲目照搬外部项目的完整依赖栈。
5. **可沉淀**：每次分析不仅给结论，也尽量提炼成未来可复用的规则。

## 主要能力

- GitHub 项目研究
- 网页与文档阅读
- 视频/社区类来源辅助判断
- 实用性评估
- adopt / adapt / avoid 决策
- 学习蒸馏与长期规则沉淀

## 参考文件

- `SKILL.md`：主路由与工作流
- `references/github.md`：GitHub 研究
- `references/web.md`：网页/文档阅读
- `references/video.md`：视频与演示材料判断
- `references/community.md`：社区信号与用户反馈
- `references/evaluation.md`：实用性评估框架
- `references/evidence-order.md`：证据优先级
- `references/output-patterns.md`：输出模板
- `references/openclaw-fit.md`：如何适配到当前 OpenClaw 工作区
- `references/research-playbooks.md`：研究流程手册
- `references/learning-distillation.md`：如何把研究变成长期能力
- `references/scoring.md`：评分卡
- `references/adoption-template.md`：落地建议模板

## 当前状态

这个技能已经通过本地结构校验，并可成功打包为 `.skill` 文件。

并且已经做过一轮本地可用性验证：

- GitHub 路径：可通过已认证的 `gh` 直接分析仓库
- 普通网页路径：适合文档/文章类来源
- 对 GitHub 页面本身，不把普通网页抓取当首选路径，而是优先 GitHub 原生访问

也就是说，这个技能不是只有“结构上合法”，而是已经验证过在当前环境里的核心路由是可用的。

如果后续继续增强，建议优先补：

- 更多真实案例样式
- 更细的 GitHub 项目分析模板
- 对不同来源（GitHub / 官网 / 文章 / 视频）的组合证据策略
