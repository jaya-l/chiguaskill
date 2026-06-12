# 🍉 chiguaskill — 吃瓜 Skill

🍉 公司 token 闲着也是闲着，不如让它帮你整理全网最新最全的瓜。覆盖微博、抖音、小红书、B站等主流社交平台。

## 两种模式

| 模式 | 触发方式 | 输出 |
|------|---------|------|
| **瓜田日报** | "最近有什么大瓜" | 热度排序的八卦事件汇总 HTML |
| **单瓜深扒** | "帮我整理 XX 事件" | 含 Mermaid 时间线图的完整脉络 HTML |

## 安装

### 方式一：通过 Claude Code 插件安装

```
/plugin marketplace add jaya-l/chiguaskill
/plugin install chiguaskill@chiguaskill
```

### 方式二：手动安装

将本仓库克隆到 Claude Code 的 skills 目录：

```bash
git clone https://github.com/jaya-l/chiguaskill.git ~/.claude/skills/chiguaskill
```

## 依赖

本 skill 是纯编排器型 skill（无需额外脚本），但依赖以下 Claude Code 内置能力：

- `web_search` — 覆盖微博、小红书、百度热搜等
- `sn-search-social-cn` — B站搜索（可选）
- `sn-md-to-html-report` — Markdown 转 HTML 报告（可选，也可直接阅读 Markdown）

## 使用示例

```
# 日报模式
"最近娱乐圈有什么大瓜？"
"帮我整理最近一周的八卦"

# 深扒模式
"帮我整理跑男最近的争议"
"XX 出轨事件是怎么回事"
```

## 输出示例

日报模式生成 HTML 报告包含：热度 TOP 5 详情、完整瓜单表格、分类统计、来源链接。

深扒模式生成 HTML 报告包含：事件概览、Mermaid 时间线图、事件阶段分析、各方回应汇总、不确定性声明。

## 行为边界

- 所有信息标注来源链接
- 区分已确认事实与网络传言
- 不编造、不传播未经核实的私密信息
- 不涉及政治敏感事件

## 许可

MIT License
