# 中文 LaTeX 排版指南：从安装到编译

> 适用场景：你想用 LaTeX 写论文但不知道从哪开始，或者编译报错了不知道怎么修。

---

## 1. LaTeX 是什么？为什么要用？

**LaTeX** 是一个排版系统——你写的是代码，它给你编译成漂亮的 PDF。

| | Word | LaTeX |
|---|------|-------|
| 学习曲线 | 低（所见即所得） | 中高（需要学语法） |
| 排版质量 | 还行，但大文档容易乱 | 专业级，尤其数学公式 |
| 参考文献 | 手动或用插件 | BibTeX 自动化（改一个样式全篇自动更新） |
| 版本管理 | 不好做（二进制文件） | 纯文本，用 Git 管理很爽 |
| 协作 | 需要 OneDrive/腾讯文档 | Overleaf 在线协作 |
| 适合什么 | 短文、非学术场景 | 学术论文、毕业论文、含有大量公式/图表/引用的文档 |

**计算机/AI 方向特别推荐 LaTeX：** 大多数 CS 会议和期刊都提供 LaTeX 模板，直接用模板省去大量排版时间。

---

## 2. 安装指南

### 选项 A：Overleaf（推荐新手）

**overleaf.com** —— 在线的 LaTeX 编辑器，不需要安装任何东西。

- 🆓 **免费版够本科论文用：** 1 个协作者、编译时长基本够（如果论文很长可以分章编译）
- 🎓 **学校邮箱可能有教育优惠**
- 优点：零安装、自动保存、模板丰富、协作方便
- 缺点：没网不能写、大文档编译慢

### 选项 B：本地安装（推荐想深入学的）

**Windows 安装步骤：**

1. 下载安装 **TeX Live**（tug.org/texlive）—— 这是 LaTeX 的"全家桶"发行版，Windows 下安装包约 4GB，装完约 8GB
2. 下载安装 **VS Code** + 安装 **LaTeX Workshop** 插件
3. 或者用 **TeXStudio**（专门的 LaTeX 编辑器，开箱即用，不用配插件）

**macOS：** 安装 MacTeX（tug.org/mactex）

**验证安装：** 打开终端，输入 `pdflatex --version`，看到版本号就说明安装成功。

---

## 3. 你的第一个 LaTeX 文档

创建一个 `test.tex` 文件，输入以下内容：

```latex
% 这是注释。% 后面的内容不会被编译。

% === 选择文档类 ===
\documentclass[12pt,a4paper]{ctexart}  % ctexart = 中文文章类
                                        % 12pt = 正文字号
                                        % a4paper = A4纸

% === 加载宏包 ===
\usepackage[UTF8]{inputenc}             % UTF-8 编码
\usepackage{amsmath,amssymb}            % 数学公式
\usepackage{graphicx}                   % 插入图片
\usepackage{booktabs}                   % 专业表格
\usepackage[hidelinks]{hyperref}        % 超链接（隐藏链接边框）

% === 标题信息 ===
\title{基于大语言模型的编程学习辅助系统}
\author{你的名字}
\date{\today}

% === 正文开始 ===
\begin{document}

\maketitle  % 生成标题页

\begin{abstract}
这是摘要内容。中文摘要通常 200-300 字。
\end{abstract}

\section{引言}
这是引言。\LaTeX{} 会自动编号和排版。

\subsection{研究背景}
这是一个子节。你不需要手动编号——LaTeX 帮你处理。

\section{方法}
这是方法部分。

\begin{equation}
    E = mc^2
    \label{eq:einstein}
\end{equation}

公式 \ref{eq:einstein} 是爱因斯坦的质能方程。

\section{结果}
结果在这里。

\section{讨论}
讨论在这里。

\section{结论}
结论在这里。

% === 参考文献 ===
\begin{thebibliography}{99}
\bibitem{example} 作者. 标题. 期刊, 年份.
\end{thebibliography}

\end{document}
```

**编译命令（终端中）：**
```bash
xelatex test.tex    # 用 XeLaTeX 编译（支持中文）
```

或者在 VS Code 中按 `Ctrl+Alt+B`（LaTeX Workshop 插件）。

---

## 4. 中文文档类选择

| 文档类 | 适合什么 | 备注 |
|--------|---------|------|
| `ctexart` | 中文期刊论文、短文 | 相当于英文的 `article` |
| `ctexrep` | 中文报告 | 相当于 `report`，章节层级更多 |
| `ctexbook` | 中文学位论文、专著 | 相当于 `book`，有 \chapter{} 命令 |

**一般用 `ctexart` 就够了（会议/期刊论文）。** 本科毕业论文用 `ctexbook`（因为你很可能需要 \chapter{}）。

---

## 5. 常见问题与修复

### 5.1 中文字体问题

**症状：** 编译后中文是乱码或者空白。

**修复：** 确保用 **XeLaTeX** 编译，不要用 pdfLaTeX。VS Code 中设置 `"latex-workshop.latex.recipe.default": "xelatex"`。

**ctex 与 xeCJK 的关系：** ctex 宏包内部会自动调用 xeCJK。**不要同时在导言区手动配置 xeCJK**——会出现双重字体定义的冲突警告。

### 5.2 中文参考文献

**推荐工具：gbt7714 宏包** —— 自动按 GB/T 7714 国家标准格式化中文参考文献。

```latex
\usepackage[backend=biber,style=gb7714-2015]{biblatex}
\addbibresource{references.bib}
```

编译顺序：
```bash
xelatex main.tex
biber main.tex       # 处理参考文献
xelatex main.tex     # 更新引用
xelatex main.tex     # 确保交叉引用完全正确
```

### 5.3 hyperref 中文书签乱码

**症状：** PDF 的书签（左侧目录）中中文显示为乱码。

**修复：**
```latex
\usepackage[CJKbookmarks=true,unicode=true]{hyperref}
```

### 5.4 算法伪代码中的中文

**在 algorithm2e 中使用中文：**

```latex
\usepackage[linesnumbered,ruled,vlined]{algorithm2e}
% 中文关键词
\SetKwInOut{Input}{输入}
\SetKwInOut{Output}{输出}
```

### 5.5 TikZ 中文标签

**在 TikZ 图片节点中使用中文：**

最简单的解决方案——在导言区设置全局字体：
```latex
\usepackage{tikz}
% ctex 已经处理了中文字体，TikZ 节点直接写中文通常可以工作
```

如果不行，尝试在 node 中指定：
```latex
\node[font=\rmfamily] {中文标签};
```

### 5.6 表格排版

专业表格的三条黄金法则：
1. 用 `booktabs` 宏包
2. **绝不用竖线**
3. 用 `\toprule`、`\midrule`、`\bottomrule`

```latex
\usepackage{booktabs}
\begin{tabular}{lccc}        % 注意：没有竖线 |
\toprule
\textbf{模型} & \textbf{准确率} & \textbf{精确率} & \textbf{召回率} \\
\midrule
BERT & 85.2 & 84.1 & 83.7 \\
GPT-4 & 92.8 & 91.5 & 90.3 \\
Ours & \textbf{94.1} & \textbf{93.2} & \textbf{92.8} \\
\bottomrule
\end{tabular}
```

### 5.7 常见编译错误速查

| 错误信息 | 可能原因 | 修复 |
|---------|---------|------|
| `Missing number, treated as zero` | ctex 版本与 LaTeX 内核冲突 | 更新 TeX Live 到最新版 |
| `Font \xxx not found` | 系统中没有对应中文字体 | Windows 一般没问题；Linux 需安装中文字体；或用 Overleaf |
| `Overfull \hbox` | 中文断行不理想 | 加 `\sloppy`（允许更多断行），或手动调整 |
| `undefined control sequence` | 拼写错误或缺失宏包 | 检查命令拼写；确认 `\usepackage{}` |
| `File 'xxx.sty' not found` | 缺少宏包 | TeX Live 自带绝大多数；用 `tlmgr install xxx` 安装 |
| `There were undefined references` | 需多次编译 | 再编译一次——交叉引用（标签/引用/参考文献）需要至少 2 遍 |
| LaTeX Error: `Environment xxx undefined` | 拼写错误 | 检查 `\begin{xxx}` 的拼写 |

---

## 6. 中文 LaTeX 模板推荐

| 模板 | 适合什么 | 获取方式 |
|------|---------|---------|
| 清华 thu-thesis | 学位论文（写得很规范，非清华学生也能参考） | GitHub 搜索 |
| 中科院 ucasthesis | 学位论文 | GitHub 搜索 |
| 上海交大 SJTUThesis | 学位论文 | GitHub 搜索 |
| 中文期刊模板 | 《计算机学报》《软件学报》《自动化学报》等 | 期刊官网下载 |

---

## 7. 复杂问题边界

当遇到以下问题时建议**查阅 CTAN 文档或 TeX Stack Exchange**，不要在聊天中死磕：

- 自定义中文文档类（修改 `.cls` 文件）
- 复杂的多语言混排（中+英+日+阿拉伯文等 > 2 种）
- 非标准字体的中文化配置
- 编译引擎切换（pdfLaTeX → XeLaTeX → LuaLaTeX）导致的兼容性问题
- 宏包之间的深层冲突（加载顺序导致的诡异 bug）

> 在 TeX Stack Exchange (tex.stackexchange.com) 上，用英文描述你的问题 + 贴出最小可复现代码 (MWE)，通常 24 小时内能拿到专业回答。
