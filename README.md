<p align="center">
  <img src="logo/dark.png" alt="RuoLi" height="60" />
</p>

<p align="center">
  <strong>RuoLi 文档</strong> — AI 模型 API 中转平台文档站
</p>

<p align="center">
  <a href="https://docs.ruoli.dev">在线文档</a> ·
  <a href="https://ruoli.dev">控制台</a> ·
  <a href="https://status.ruoli.dev/status/all">服务状态</a>
</p>

---

## 关于

[RuoLi](https://ruoli.dev) 是一个统一的 AI 模型 API 中转平台。一个 API Key，通过 OpenAI 兼容接口访问 Claude、GPT、Gemini、Deepseek 等主流大模型。

本仓库是 RuoLi 的文档站源码，基于 [Mintlify](https://mintlify.com) 构建，支持中英双语。

## 文档内容

- **快速开始** — 注册账号、获取 API Key
- **平台使用** — 模型分组、定价倍率、充值计费
- **配置工具** — CC Switch、Claude Code、Codex、Gemini CLI、OpenCode、OpenClaw、Cherry Studio 的接入教程

## 项目结构

```text
ruoli-docs/
├── docs.json                  # Mintlify 配置
├── index.mdx                  # 介绍（中文）
├── quickstart.mdx             # 快速开始（中文）
├── platform/                  # 平台使用（中文）
│   ├── models-and-groups.mdx
│   ├── billing.mdx
│   └── faq.mdx
├── tools/                     # 配置工具（中文）
│   ├── cc-switch.mdx
│   ├── claude-code.mdx
│   ├── codex.mdx
│   ├── gemini-cli.mdx
│   ├── opencode.mdx
│   ├── openclaw.mdx
│   └── cherry-studio.mdx
├── en/                        # 英文版（镜像结构）
├── logo/                      # 品牌素材
└── images/                    # 截图
```

## 本地开发

> [!NOTE]
> 需要 Node.js 22（LTS）。Mintlify CLI 不支持 Node 25+。

```bash
npm i -g mint
mint dev
```

如果默认 Node 是 25+，使用 Node 22：

```bash
PATH="/opt/homebrew/opt/node@22/bin:$PATH" mint dev
```

预览地址：[http://localhost:3000](http://localhost:3000)

## 发布

推送到 `main` 分支后，通过 [Mintlify GitHub App](https://dashboard.mintlify.com/settings/organization/github-app) 自动部署。

## MCP 服务

AI 工具可通过 MCP 连接文档：

```
https://docs.ruoli.dev/mcp
```

可用工具：`search_ruoli`、`get_page_ruoli`。
