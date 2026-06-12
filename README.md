 # 🍉 chiguaskill —吃瓜 Skill

  🍉 公司 token 闲着也是闲着，不如让它帮你整理全网最新最全的瓜。覆盖微博、抖音、小红书、B站等主流社交平台。

  ## 两种模式

  | 模式 | 触发方式 | 输出 |
  |------|---------|------|
  | **瓜田日报** | "最近有什么大瓜" | 热度排序的八卦事件汇总 HTML |
  | **单瓜深扒** | "帮我整理 XX 事件" | 含 Mermaid 时间线图的完整脉络 HTML |

  ## 安装

  /plugin marketplace add jaya-l/chiguaskill
  /plugin install sn-chigua@sn-chigua


  ## 依赖

  - `web_search` — 覆盖微博、小红书、百度热搜等
  - `sn-search-social-cn` — B站搜索（可选）
  - `sn-md-to-html-report` —Markdown 转 HTML 报告（可选）

  ## 使用示例

  "最近娱乐圈有什么大瓜？"
  "帮我整理跑男最近的争议"

  ## 行为边界

  - 所有信息标注来源链接
  - 区分已确认事实与网络传言
  - 不编造、不传播未经核实的私密信息
  - 不涉及政治敏感事件

  ## 许可

  MIT License
