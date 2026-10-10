<div align="center">

# Hi, I'm gus 👋 · 你好，我是 gus

**Java backend engineer → AI Agent engineer**
**Java 后端工程师，正在转型 AI Agent 工程**

Open-source contributor to LangChain4j, SpotBugs, DeerFlow and more.
LangChain4j、SpotBugs、DeerFlow 等开源项目的贡献者。

</div>

---

## 🧭 About · 关于我

- 🔭 Building LLM-powered applications on the JVM: agents, RAG, tool calling, MCP.
  专注在 JVM 上构建基于大模型的应用：Agent、RAG、工具调用、MCP。
- 🌱 Learning in public by contributing to the projects I use, mainly [LangChain4j](https://github.com/langchain4j/langchain4j).
  通过给自己在用的项目提交代码来学习，主要是 LangChain4j。
- 💬 Ask me about: Java, Spring, LangChain4j, Redis, Kafka.
  可以和我聊：Java、Spring、LangChain4j、Redis、Kafka。

---

## 🏆 Merged Contributions · 已合并的贡献

Source-code contributions with tests, merged into widely used open-source projects.
均为带测试的源码贡献，已合并进广泛使用的开源项目。

### [LangChain4j](https://github.com/langchain4j/langchain4j) ![stars](https://img.shields.io/github/stars/langchain4j/langchain4j?style=flat&logo=github)

| PR | What it does · 内容 |
|---|---|
| [#5690](https://github.com/langchain4j/langchain4j/pull/5690) | **Structured outputs for numeric parsers.** Added `jsonSchema()` to the Byte/Short/BigInteger/BigDecimal output parsers so they match Integer/Long/Float/Double.<br>**数值类输出解析器支持结构化输出**：为 Byte/Short/BigInteger/BigDecimal 补上 `jsonSchema()`，与其他数值解析器对齐。 |
| [#5880](https://github.com/langchain4j/langchain4j/pull/5880) | **Config escape hatch for Google GenAI batch model.** Added `generateContentConfigCustomizer` to `GoogleGenAiBatchChatModel`, completing the option already available on the sync and streaming models.<br>**Google GenAI 批量模型配置定制**：补齐同步、流式模型已有的底层参数定制入口。 |
| [#5924](https://github.com/langchain4j/langchain4j/pull/5924) | **Fix A2A hang on interrupted tasks.** When a remote agent enters `input-required` / `auth-required`, the response future now completes exceptionally (new `A2ATaskInterruptedException`) instead of hanging forever.<br>**修复 A2A 任务中断时的挂起**：任务进入 `input-required` / `auth-required` 时，响应 future 以异常结束，不再一直等待。 |
| [#6021](https://github.com/langchain4j/langchain4j/pull/6021) | **Fix garbled error messages.** `ApacheHttpClient` decoded error bodies with the JVM default charset and rewrote line separators; now reads UTF-8 and preserves them.<br>**修复错误信息乱码**：错误响应体改用 UTF-8 读取并保留原始换行，不再依赖 JVM 默认字符集。 |

### [SpotBugs](https://github.com/spotbugs/spotbugs) ![stars](https://img.shields.io/github/stars/spotbugs/spotbugs?style=flat&logo=github)

| PR | What it does · 内容 |
|---|---|
| [#4288](https://github.com/spotbugs/spotbugs/pull/4288) | **Fix a false positive in resource-leak detection.** `writer = writer.append(...)` made `FindOpenStream` report a leak even when the writer was closed in `finally`; the stream-modeling visitor now preserves the receiver's resource identity for the `PrintWriter.append` overloads, and only for `PrintWriter` itself so subclass overrides are not misjudged.<br>**修复资源泄漏检测的误报**：`PrintWriter.append` 之后资源标识丢失导致误报，现保留接收者的资源标识，并限定只对 `PrintWriter` 本身生效，避免误判子类重写。 |

### [DeerFlow](https://github.com/bytedance/deer-flow) ![stars](https://img.shields.io/github/stars/bytedance/deer-flow?style=flat&logo=github)

| PR | What it does · 内容 |
|---|---|
| [#5111](https://github.com/bytedance/deer-flow/pull/5111) | **Make the sandbox agent inspect, not guess.** With host Bash enabled, the agent now probes the real environment (`uname -s`, `sw_vers`, …) and gets actionable guidance when a host path is blocked, instead of repeating the same rejected probe.<br>**让沙箱 agent 以工具证据而非假设作答**：按真实命令探测运行环境，宿主机路径被拦截时给出可执行的替代指引，避免重复同一个被拒绝的探测。 |

### 🔄 In review · 审核中

- [openrewrite/rewrite#8779](https://github.com/openrewrite/rewrite/pull/8779): Allow overriding Maven plugin versions managed by external parents · 允许覆盖由外部父 POM 管理的 Maven 插件版本
- [langchain4j/langchain4j#6103](https://github.com/langchain4j/langchain4j/pull/6103): Handle UUID-as-string in range metadata filters · 范围元数据过滤器支持字符串形式的 UUID
- [spring-projects/spring-ai#6407](https://github.com/spring-projects/spring-ai/pull/6407): Add guide for building a console application · 新增控制台应用构建指南

> All merged PRs: [search link · 全部已合并 PR](https://github.com/pulls?q=is%3Apr+author%3Aangus-guo+is%3Amerged+-user%3Aangus-guo)

---

## 🚀 Projects · 我的项目

| Project | Description · 简介 |
|---|---|
| [gps-code](https://github.com/angus-guo/gps-code) | A Chinese-first TUI code agent that helps developers understand unfamiliar codebases, with read-only tools, confirmed command execution and diff-previewed safe edits · 中文优先的 TUI code agent，帮助理解陌生代码库，支持只读检索、确认后执行命令、带 diff 预览的安全编辑 |
| [dsh-deepseek-balance](https://github.com/angus-guo/dsh-deepseek-balance) | DeepSeek balance and session cost plugin for the dsh web GUI · dsh 网页界面的 DeepSeek 余额与会话成本插件 |
| [poem4u](https://github.com/angus-guo/poem4u) | Chinese poem generator (Spring Boot + TypeScript) that validates line count, character count and name coverage before returning · 中文诗词生成应用，返回前校验行数、字数与嵌字要求 |
| [claude-key-panel](https://github.com/angus-guo/claude-key-panel) | Visual panel for managing and switching multiple Claude keys · 管理切换多个 Claude key 的可视化面板 |
| [whack-a-wole](https://github.com/angus-guo/whack-a-wole) | Whack-a-mole web game in pure HTML/CSS/JS with 10 levels · 纯前端打地鼠小游戏，共 10 关 |

---

## 🛠️ Tech Stack · 技术栈

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**AI Agent**

![LangChain4j](https://img.shields.io/badge/LangChain4j-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langgraph&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

**Frontend · 前端**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

---

## 📊 GitHub Stats · 统计

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=angus-guo&show_icons=true&count_private=true&include_all_commits=true&hide_border=true" alt="GitHub stats" />
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=angus-guo&layout=compact&hide_border=true" alt="Top languages" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=angus-guo&hide_border=true" alt="Streak" />

</div>

---

## 📫 Contact · 联系

- GitHub: [@angus-guo](https://github.com/angus-guo)
- Email: 1721581427@qq.com
