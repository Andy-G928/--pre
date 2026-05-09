# Advanced Microeconomics Presentation

本项目是高级微观经济学博士课程的 40 分钟小组汇报 slides。汇报论文为 Hagiu, Teh, and Wright (2022), "Should Platforms Be Allowed to Sell on Their Own Marketplaces?"，汇报时间为 2026 年 5 月 18 日。

slides 正文使用英文。中文可以用于 README、协作说明、个人笔记和讨论记录，但不要写进正式 slides 页面。

## 项目目标

我们需要共同完成一套 LaTeX Beamer slides，详细介绍论文的核心故事、理论模型、均衡分析、福利含义和政策结论。

本次汇报的重点不是简单复述文章，而是把论文中的模型建立、分析逻辑、求解步骤和经济学直觉讲清楚。听众是中国学生，因此 slides 英文应尽量清楚、简单，避免使用过难词汇；如果是论文中已经出现的专业词，可以保留。

## 文件结构

主要文件如下：

```text
.
|-- README.md
|-- AGENTS.md
|-- notebook.md
|-- presentation_framework.md
|-- The RAND J of Economics - 2022 - Hagiu - Should platforms be allowed to sell on their own marketplaces.md
|-- The RAND J of Economics - 2022 - Hagiu - Should platforms be allowed to sell on their own marketplaces.pdf
`-- slides
    |-- demo.tex
    |-- demo.pdf
    |-- tex
    |   |-- 01_research_question.tex
    |   |-- 02_baseline_model.tex
    |   |-- 03_equilibrium_analysis.tex
    |   |-- 04_ban_on_dual_mode.tex
    |   `-- 05_policy_and_extensions.tex
    |-- image
    |-- beamerthemelingnan.sty
    |-- beamerouterthemelingnan.sty
    |-- beamerinnerthemelingnan.sty
    `-- beamercolorthemelingnan.sty
```

最重要的入口文件是：

```text
slides/demo.tex
```

五个人分别修改 `slides/tex/` 目录下的五个文件。一般情况下，不需要直接修改 `slides/demo.tex`，也不要修改 `.sty` 模板文件。

## 五个人的分工

### 第 1 位：Research Question

负责文件：

```text
slides/tex/01_research_question.tex
```

负责内容：

- 介绍平台自营与第三方卖家的现实问题。
- 解释论文要回答的核心问题：平台是否应该被允许在自己的 marketplace 上销售自营产品。
- 说明为什么这个问题涉及 self-preferencing、competition、consumer welfare 和 platform incentives。
- 概括文章的主要贡献和汇报路线。

写作目标：

- 让听众知道这篇文章为什么重要。
- 不要过早进入复杂公式。
- 需要为后面的模型部分铺垫直觉。

### 第 2 位：Baseline Model

负责文件：

```text
slides/tex/02_baseline_model.tex
```

负责内容：

- 介绍 baseline model 的参与者：platform、third-party sellers、consumers。
- 说明时间顺序和每一阶段谁做什么决策。
- 定义主要变量、价格、佣金、进入决策、搜索或排序机制等。
- 解释平台 dual mode 的含义：既是 marketplace operator，也是 seller。

写作目标：

- 模型设定必须完整，因为后面的均衡分析都依赖这一部分。
- 每个变量第一次出现时都要解释。
- 每个假设后面最好补一句经济学直觉：这个假设为什么合理，它简化了什么问题。

### 第 3 位：Equilibrium Analysis

负责文件：

```text
slides/tex/03_equilibrium_analysis.tex
```

负责内容：

- 推导 baseline model 中的均衡。
- 解释平台、第三方卖家和消费者的最优反应。
- 展示关键 proposition、lemma 或 equilibrium condition。
- 分析平台什么时候选择进入、什么时候不进入。
- 解释每个数学结果背后的经济学机制。

写作目标：

- 这是整场汇报的核心之一。
- 不要只给结论，要展示关键求解步骤。
- 公式后面要有 intuition，帮助听众理解公式在说什么。
- 如果推导太长，可以拆成多页 slides。

### 第 4 位：Ban on Dual Mode

负责文件：

```text
slides/tex/04_ban_on_dual_mode.tex
```

负责内容：

- 分析禁止平台自营后的市场结果。
- 对比允许 dual mode 和禁止 dual mode 时的均衡变化。
- 说明第三方卖家的进入、定价、平台佣金或消费者选择如何改变。
- 解释 ban 的收益和成本。

写作目标：

- 不只是说 ban 好或不好，而是说明为什么。
- 重点放在机制比较：平台不能自营后，激励结构如何变化。
- 尽量用表格或简单对比页展示两个制度的差别。

### 第 5 位：Policy and Extensions

负责文件：

```text
slides/tex/05_policy_and_extensions.tex
```

负责内容：

- 介绍福利分析：consumer surplus、seller profit、platform profit、total welfare。
- 总结论文对平台监管的政策含义。
- 介绍文章中的扩展或 robustness analysis。
- 给出结论：什么时候允许平台自营可能有益，什么时候可能有害。

写作目标：

- 把理论结果和现实政策问题连接起来。
- 不要把政策结论讲成单一答案；这篇文章的关键在于条件和机制。
- 最后一页要帮助全组收束：paper 的 main message 是什么。

## 每个人应该怎么做

### 1. 先读材料

推荐阅读顺序：

1. 先看 `notebook.md`，快速理解论文故事。
2. 再看 `presentation_framework.md`，理解我们准备怎么讲。
3. 然后读论文转换后的 Markdown：

```text
The RAND J of Economics - 2022 - Hagiu - Should platforms be allowed to sell on their own marketplaces.md
```

4. 如果 Markdown 中公式、图表或命题不清楚，再回到原始 PDF 核对。

### 2. 只改自己负责的 tex 文件

为了减少 Git 冲突，每个人主要修改自己的文件：

```text
slides/tex/01_research_question.tex
slides/tex/02_baseline_model.tex
slides/tex/03_equilibrium_analysis.tex
slides/tex/04_ban_on_dual_mode.tex
slides/tex/05_policy_and_extensions.tex
```

不要随便修改这些文件：

```text
slides/demo.tex
slides/*.sty
slides/image/*
```

如果确实需要修改主文件、模板或图片，先在群里说明，避免多人同时改同一个文件。

### 3. 每页 slide 的建议写法

每页 slide 尽量遵守：

- 标题清楚，说明这一页回答什么问题。
- bullet points 不要太长。
- 公式不要堆太多，一页只讲一个主要结果。
- 重要公式后面加一句 `Intuition:`。
- 如果是 proposition 或 conclusion，最好拆成 `Result` 和 `Intuition` 两部分。
- 英文尽量简单，适合课堂汇报时口头解释。

示例：

```tex
\begin{frame}{Platform Entry Decision}
  \begin{block}{Result}
    The platform enters when its gain from direct sales is larger than the loss from lower third-party seller profit.
  \end{block}

  \begin{block}{Intuition}
    Entry creates a new profit source for the platform, but it may also reduce the value of the marketplace for outside sellers.
  \end{block}
\end{frame}
```

## 如何编译 slides

本项目使用 XeLaTeX 编译。建议使用 TeX Live 或 MiKTeX。

在终端进入 `slides/` 目录：

```powershell
cd slides
```

然后运行：

```powershell
xelatex -synctex=1 "demo.tex"
```

如果目录、页码或交叉引用没有更新，再运行一次：

```powershell
xelatex -synctex=1 "demo.tex"
```

编译成功后会生成：

```text
slides/demo.pdf
```

如果你只修改了自己的 section 文件，也需要编译 `demo.tex`，因为 `demo.tex` 是整套 slides 的主入口。

## GitHub 新手协作流程

### 第一次下载项目

如果你还没有本地项目，先 clone：

```powershell
git clone <repository-url>
cd <repository-folder>
```

如果你已经有本地项目，每次开始写之前先同步最新版本：

```powershell
git pull
```

### 修改前先创建自己的分支

建议每个人用自己的分支，不要直接在 `main` 分支上改：

```powershell
git checkout -b name-section
```

例如：

```powershell
git checkout -b zhang-baseline-model
```

### 查看自己改了哪些文件

写完后先查看状态：

```powershell
git status
```

再查看具体改动：

```powershell
git diff
```

确认只改了自己负责的文件后，再提交。

### 提交自己的修改

把文件加入暂存区：

```powershell
git add slides/tex/02_baseline_model.tex
```

提交：

```powershell
git commit -m "Draft baseline model section"
```

推送到 GitHub：

```powershell
git push origin zhang-baseline-model
```

然后在 GitHub 上创建 Pull Request，请其他组员检查后再合并。

## 不要提交的文件

LaTeX 编译会生成很多中间文件，例如：

```text
.aux
.log
.nav
.out
.snm
.synctex.gz
.toc
```

这些文件已经在 `.gitignore` 中忽略。一般只需要保留：

```text
slides/demo.tex
slides/demo.pdf
slides/tex/*.tex
```

如果发现中间文件出现在 GitHub 的改动列表中，不要提交它们。可以先运行：

```powershell
git status
```

确认哪些文件被跟踪。如果不确定，先在群里问。

## 合并前检查清单

每个人提交前请检查：

- 自己负责的部分是否完整。
- 是否可以成功编译 `slides/demo.tex`。
- slides 正文是否为英文。
- 重要数学结果是否有经济学直觉解释。
- 是否没有使用过难英文词汇。
- 是否没有随意修改别人的 section。
- 是否没有提交 LaTeX 中间文件。
- 是否没有把中文写进正式 slide 页面。

全组合并前请检查：

- 5 个 section 的逻辑是否连贯。
- 总页数和内容量是否适合 40 分钟。
- 模型设定、均衡分析、政策含义是否前后统一。
- 符号是否一致。
- 相同概念是否使用同一个英文表达。
- `slides/demo.pdf` 是否是最新编译结果。

## 常见问题

### 我应该改哪个文件？

只改你负责的 `slides/tex/0x_*.tex` 文件。不要直接改 `demo.pdf`，PDF 是编译生成的。

### 我改完 tex 后为什么 PDF 没变？

需要重新编译：

```powershell
cd slides
xelatex -synctex=1 "demo.tex"
```

### 我不懂 LaTeX 怎么办？

可以先模仿已有页面的结构。最常用的是：

```tex
\begin{frame}{Slide Title}
  \begin{itemize}
    \item First point.
    \item Second point.
  \end{itemize}
\end{frame}
```

如果要写公式：

```tex
\[
  \pi = p q - c(q)
\]
```

如果要强调结果：

```tex
\begin{block}{Intuition}
  The platform trades off direct sales profit against the effect on third-party sellers.
\end{block}
```

### 出现冲突怎么办？

如果 GitHub 提示 conflict，不要慌。通常是两个人改了同一个文件。先停止合并，在群里说明冲突文件名，再由其中一人手动合并内容。

减少冲突的最好方法是：每个人只改自己的 section 文件。

## 推荐协作节奏

1. 每个人先完成自己 section 的第一版。
2. 全组一起读一遍 `demo.pdf`，检查逻辑是否连贯。
3. 第 2 位和第 3 位重点统一模型符号和求解逻辑。
4. 第 4 位和第 5 位重点统一政策比较和福利分析。
5. 最后统一格式、页数、英文表达和讲稿节奏。

建议最后至少预留一次完整排练。40 分钟汇报中，每个人平均大约 8 分钟，但模型和均衡部分可能需要更多时间，可以根据实际内容再调整。
