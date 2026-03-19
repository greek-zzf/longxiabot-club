# 🦞 OpenClaw (龙虾) 中文本地部署指南与报错求助专区

[![Official Site](https://img.shields.io/badge/主站-龙虾俱乐部_(longxiabot.club)-eb4f34?style=for-the-badge)](https://longxiabot.club)
[![Skill Hub](https://img.shields.io/badge/资源-100%2B_中文_Skill_插件库-blue?style=for-the-badge)](https://longxiabot.club/skills)

欢迎来到 **龙虾俱乐部 (LongxiaBot Club)** 的官方 GitHub 交流仓库！

本仓库主要用于 **OpenClaw (龙虾) AI 智能体** 的中文本地化文档存档、常见报错反馈（Issues）以及新手答疑。由于开源生态的 Skill 插件更新极快，**最新、最完整的图文教程与开箱即用的配置文件，请统一前往我们的主站获取。**

👉 **[点击访问：龙虾俱乐部 (longxiabot.club) - 全网最全的 OpenClaw 中文实战大本营](https://longxiabot.club)**

---

## 🚀 核心导航 (快速直达主站)

- 📖 **[零基础保姆级部署教程 (Windows/macOS)](https://longxiabot.club/getting-started)**
- 🧩 **[中文 Skill 插件市场 (接入微信/飞书/推特等)](https://longxiabot.club/skills)**
- ⚡ **[API 与本地大模型配置指南 (低显存优化)](https://longxiabot.club/docs/models/provider-overview)**
- 🚨 **[常见报错排查字典 (解决显存不足、网络超时等)](https://longxiabot.club/docs/appendix/faq)**

---

## 🛠️ 试读：OpenClaw 常见环境报错速查

*(以下内容节选自龙虾俱乐部教程库，完整版请访问主站)*

### 1. 运行 `openclaw hatch` 时提示网络连接超时？
这通常是因为拉取依赖时 GitHub 或外网镜像被墙。
**解决方案：** 请确保你的终端（Terminal/PowerShell）已开启全局代理。
Windows 环境下，可在终端执行：
```powershell
set http_proxy=[http://127.0.0.1](http://127.0.0.1):你的端口
set https_proxy=[http://127.0.0.1](http://127.0.0.1):你的端口
```
💡 完整代理配置与国内镜像源替换教程，请查看：网络配置终极指南

### 2. 报错 CUDA out of memory？
你的显存不足以运行当前的本地开源大模型。
**解决方案：**
如果你只有 8G 或更低的显存，强烈建议切换为调用云端 API（如 Kimi、智谱或 Claude），对本地显卡零要求。
💡 如何修改 config.yaml 接入国内免费大模型 API？请查看：低配置电脑运行方案

## 💬 提问与求助 (Issues 规则)
如果你在本地部署 OpenClaw 或安装 Skill 时遇到了本仓库及主站未能解决的奇葩报错，欢迎在 Issues 面板 中提出。

## 声明
本仓库及龙虾俱乐部仅提供 OpenClaw 开源框架的技术交流与配置教程。我们不提供任何大型语言模型（LLM）的直接下载服务，请用户在遵守当地法律法规的前提下，合法合规地使用相关 AI 技术与服务。
