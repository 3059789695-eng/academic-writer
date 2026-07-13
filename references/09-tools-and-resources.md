# 科研工具清单

> 这是给本科生的实用工具推荐。每一个都标注了免费情况——标 🆓 的免费、标 🎓 的学校可能已付费。

---

## 1. 文献管理

| 工具 | 特点 | 费用 |
|------|------|------|
| **Zotero** | 开源免费、浏览器插件一键抓取论文元数据、支持 BibTeX/GB7714 导出、支持协作 | 🆓 完全免费 |
| **EndNote** | 功能强大、Word 插件好用 | 🎓 去学校图书馆网站查 campus license |
| **Mendeley** | PDF 管理 + 文献管理 | 🆓 免费版够用 |

> **推荐 Zotero。** 安装 → 浏览器装 Zotero Connector 插件 → 在知网/Google Scholar 点一下就能自动保存文献信息。

---

## 2. 文献检索

| 工具 | 地址 | 特点 | 费用 |
|------|------|------|------|
| **知网 (CNKI)** | cnki.net | 中文文献首选 | 🎓 校内 IP 免费下载 |
| **万方** | wanfangdata.com.cn | 中文文献补搜 | 🎓 校内 IP 免费下载 |
| **Google Scholar** | scholar.google.com | 英文文献搜索最方便 | 🆓 免费 |
| **Semantic Scholar** | semanticscholar.org | AI 驱动、引用图谱、AI 领域特别好用 | 🆓 免费 |
| **arXiv** | arxiv.org | CS/AI 预印本、最新研究 | 🆓 免费 |
| **DBLP** | dblp.org | 计算机领域专用索引 | 🆓 免费 |
| **Web of Science** | webofscience.com | 高影响力论文筛选 | 🎓 学校图书馆 |
| **Connected Papers** | connectedpapers.com | 输入一篇论文→生成关联文献图谱 | 🆓 免费版每天几次查询够用 |

---

## 3. 写作工具

### LaTeX

| 工具 | 特点 | 费用 |
|------|------|------|
| **Overleaf** | 在线 LaTeX 编辑器，可以协作，模板丰富 | 🆓 免费版 1 个协作者、编译时长基本够本科论文 |
| **VS Code + LaTeX Workshop** | 本地写 LaTeX 最舒服的组合 | 🆓 免费 |
| **TeXStudio** | 专门的 LaTeX IDE，开箱即用 | 🆓 免费 |
| **TeX Live** | LaTeX 发行版（全家桶） | 🆓 免费 |

> Overleaf 免费版限制：1 个协作者、每次编译有时长限制。本科论文够用——如果论文很长可以分章编译。

### Word

| 工具 | 特点 | 费用 |
|------|------|------|
| **Microsoft Word** | 学校通常提供 Office 365 教育版 | 🎓 用学校邮箱注册 |

---

## 4. 语法检查与写作辅助

| 工具 | 特点 | 费用 |
|------|------|------|
| **Grammarly** | 英文语法+风格检查，学术模式 | 🎓 很多大学买了 Premium，用学校邮箱注册试试 |
| **DeepL Write** | AI 驱动的英文润色改写 | 🆓 免费版每天有额度 |
| **DeepL Translate** | 中→英翻译质量普遍被认为比 Google Translate 好 | 🆓 免费版每天有额度 |

---

## 5. 图表绘制

| 工具 | 适合什么 | 费用 |
|------|---------|------|
| **Python matplotlib + seaborn** | 折线图/柱状图/散点图/热力图 | 🆓 免费开源 |
| **Python plotly** | 交互式图表 | 🆓 免费开源 |
| **R ggplot2** | 统计图表（社科常用） | 🆓 免费开源 |
| **draw.io** | 流程图/架构图/系统设计图 | 🆓 免费 |
| **Visio** | 流程图（Word 用户友好） | 🎓 部分学校有 license |
| **Figma** | UI/交互设计图 | 🆓 免费版够用 |

> AI 论文的**模型架构图**可以用 draw.io 手绘，也可以用 Python 的 `diagrams` 库自动生成，还可以用 TikZ（LaTeX 原生的矢量图绘制方式——画出来的图是 PDF 矢量图，永远不会模糊）。

---

## 6. 公式编辑

| 工具 | 特点 | 费用 |
|------|------|------|
| **LaTeX 公式** | 最美观的公式排版 | 🆓 免费 |
| **MathType** | Word 公式插件 | 🎓 部分学校有 license |

---

## 7. 版本管理（强烈推荐）

| 工具 | 特点 | 费用 |
|------|------|------|
| **Git + GitHub** | 代码 + 论文都可以版本管理 | 🆓 免费 |
| **Git + Gitee（码云）** | GitHub 的国内替代 | 🆓 免费 |

> 论文用 Git 管起来：每次大改前 commit，改坏了可以回退。LaTeX（纯文本）+ Git = 完美组合。

---

## 8. 💡 隐藏福利：GitHub Student Developer Pack

**用学校 .edu 邮箱认证学生身份，就可以免费获得：**

| 福利 | 价值 | 用途 |
|------|------|------|
| **JetBrains 全家桶** | ~$649/年 | PyCharm、IntelliJ IDEA、WebStorm 等全部 IDE 免费 |
| **GitHub Copilot** | ~$100/年 | AI 辅助编程（你用的 Claude Code 也是极佳的 Coding Agent 选择） |
| **GitHub Pro** | ~$48/年 | 无限私有仓库 |
| **DigitalOcean** | $200 额度 | 云服务器，跑实验/搭服务 |
| **Namecheap** | 1 年免费域名 + SSL | 搭个人网站/博客 |
| **Canva Pro** | ~$155/年 | 做学术海报 (Poster) / 汇报 PPT |
| **更多 100+ 福利** | | 去 education.github.com/pack 查看 |

> **申请方法：** 去 education.github.com → 用学校邮箱注册 → 上传学生证或学信网截图 → 等审核（通常 1-7 天）。

---

## 9. 从哪开始？按优先级推荐

如果你是第一次接触这些工具，推荐按这个顺序来：

**第一优先级（马上开始用）：**
1. **Zotero** — 文献管理，从现在开始每读一篇就存一篇
2. **Google Scholar + Semantic Scholar** — 找英文文献
3. **知网（通过学校图书馆）** — 找中文文献

**第二优先级（写作时用）：**
4. **Overleaf** — 如果你用 LaTeX 写作
5. **Grammarly** — 英文语法检查（用学校邮箱登陆）
6. **DeepL** — 中译英第一选择

**第三优先级（锦上添花）：**
7. **GitHub Student Developer Pack** — 先申请，审批需要时间
8. **draw.io** — 画流程图/架构图
9. **Git** — 管理论文版本
