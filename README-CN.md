# Claude Code 中文版

> **更好的工具管理，而不仅仅是存储泄露的 Claude Code 档案**

这是 [instructkr/claude-code](https://github.com/instructkr/claude-code) 的中文版本。

## 关于这个项目

2026 年 3 月 31 日凌晨 4 点，作者被电话吵醒——Claude Code 源码泄露，整个开发社区沸腾了。作者的韩国女友真的担心他会因机器上有这段代码而面临 Anthropic 的法律诉讼——所以在压力下，作者做了任何工程师都会做的事情：坐下来，从零开始将核心功能移植到 Python，并在太阳升起前推送代码。

整个流程是通过 [oh-my-codex (OmX)](https://github.com/Yeachan-Heo/oh-my-codex) 由 [@bellman_ych](https://x.com/bellman_ych) 端到端编排完成的——这是一个构建在 OpenAI 的 Codex ([@OpenAIDevs](https://x.com/OpenAIDevs)) 之上的工作流层。作者使用 `$team` 模式进行并行代码审查，使用 `$ralph` 模式进行持续执行循环和架构级验证。整个移植会话——从读取原始 harness 结构到生成带测试的可用 Python 树——都是通过 OmX 编排驱动的。

结果是一个干净室的 Python 重写，捕捉了 Claude Code agent harness 的架构模式，而没有复制任何专有源代码。

## 项目特点

- 🚀 **纯 Python 实现**：完全用 Python 编写的 Agent Harness 框架
- 🧠 **智能工具管理**：不仅仅是存储代码，而是提供强大的工具编排能力
- 🔧 **模块化设计**：清晰的架构，易于扩展和维护
- 📚 **丰富的工具集**：内置多种开发工具和命令

## 快速开始

### 安装依赖

```bash
pip install -r requirements.txt
```

### 运行

```bash
python src/main.py
```

## 项目结构

```
claude-code-fork/
├── src/
│   ├── main.py          # 主入口
│   ├── runtime.py       # 运行时核心
│   ├── commands.py      # 命令系统
│   ├── query_engine.py  # 查询引擎
│   └── ...              # 其他模块
├── README.md            # 英文文档
└── README-CN.md         # 中文文档（本文件）
```

## 贡献

欢迎提交 Issue 和 Pull Request！

## 许可证

遵循原项目许可证。

## 致谢

- 原项目：[instructkr/claude-code](https://github.com/instructkr/claude-code)
- 工作流工具：[oh-my-codex](https://github.com/Yeachan-Heo/oh-my-codex)
