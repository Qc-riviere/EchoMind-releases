<div align="center">

# EchoMind · 灵感笔记

**「灵感笔记」+ 微信原生 + 本地优先**

跨设备的第二大脑——桌面速记、手机微信落库、AI 自动整理、本地优先存储。

[![Latest Release](https://img.shields.io/github/v/release/Qc-riviere/EchoMind-releases?label=最新版本&color=adc7ff)](https://github.com/Qc-riviere/EchoMind-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/Qc-riviere/EchoMind-releases/total?label=下载量)](https://github.com/Qc-riviere/EchoMind-releases/releases)
[![Platform](https://img.shields.io/badge/平台-Windows%20%7C%20macOS-blue)](https://github.com/Qc-riviere/EchoMind-releases/releases/latest)

[**📥 下载最新版**](https://github.com/Qc-riviere/EchoMind-releases/releases/latest) ·
[**💬 提交反馈**](https://github.com/Qc-riviere/EchoMind-releases/issues/new) ·
[**📖 使用文档**](./docs/getting-started.md)

</div>

---

## 这是什么

EchoMind 是一款定位为「灵感笔记」的桌面 + 微信跨端 App：

- **桌面端**（Windows / macOS）：全局热键 `Ctrl+Shift+I` 唤出浮窗 → Enter 落库 → Esc 隐藏。一切操作 200ms 内可见。
- **微信端**：通过腾讯官方 ClawBot 桥接，手机微信直接发消息即可记录灵感，桌面 ~5 秒内同步并通知。
- **AI 加工**：自动 enrich（领域 / 标签 / 上下文）、单条对话深挖、多选灵感一键总结，三格式（MD / DOCX / PDF）导出。
- **本地优先**：默认全部数据在本机 SQLite 库；云端是明确可选项。
- **BYO Key**：自带 LLM API Key（OpenAI / Claude / Gemini / DeepSeek 任选）+ 可选预算硬上限。

## 为什么选 EchoMind

| 我用过…… | 但是…… | EchoMind 怎么解 |
|---|---|---|
| Notion / 语雀 | 数据在别人的云上，断网不能用 | 本地优先，离线照常运转 |
| Obsidian | 装插件配置太复杂，没微信入口 | 开箱即用，原生支持微信落库 |
| Flomo | 没有 AI 加工，只能存不能想 | 内置多 LLM 深挖 + 总结 + 导出 |
| ChatGPT / 微信收藏 | 内容散在群和聊天里翻不到 | 语义检索 + 思维图谱可视化关联 |

## 下载安装

→ [**前往最新版本下载页**](https://github.com/Qc-riviere/EchoMind-releases/releases/latest)

| 平台 | 包名 | 安装提示 |
|---|---|---|
| Windows 10/11 (x64) | `EchoMind_x.y.z_x64-setup.exe` | 双击安装；首次启动 SmartScreen 拦截 → 点「更多信息」→「仍要运行」|
| macOS (Intel + Apple Silicon) | `EchoMind_x.y.z_universal.dmg` | 拖入 Applications；首次启动 Gatekeeper 拦截 → **右键 →「打开」→ 再次「打开」**（v0.2 暂未做 Apple 签名）|

## 5 分钟上手

1. **首次启动** → 4 步向导自动弹出（DeepSeek API Key 最低门槛 ¥10 即可）
2. **桌面速记** → 任意位置按 `Ctrl+Shift+I` 唤出浮窗，输入 → Enter 保存
3. **微信桥**（可选） → 侧栏「微信桥」→ 扫码绑定，手机微信发消息即落库
4. **AI 深挖** → 任一灵感卡片 → 「对话」按钮 → 多轮拷问
5. **批量总结** → 主列表卡片右上 ⋯ hover 即变 ☐，勾选 2-20 条 → 底栏「AI 总结」→ 导出 PDF

详细教程：[docs/getting-started.md](./docs/getting-started.md)

## 核心功能

<table>
<tr>
<td width="50%">

**📝 灵感记录**
- 全局热键速记浮窗
- 系统托盘常驻 + 今日新增徽标
- 微信 Bot 原生落库
- AI 自动补全（上下文 / 领域 / 标签）

**🧠 AI 加工**
- 单条对话深挖（多 LLM 提供商）
- 多选 AI 总结（2–20 条一次）
- 三格式导出（MD / DOCX / PDF）
- App 内置 Agent + 工具调用 loop

</td>
<td width="50%">

**🔍 检索与关联**
- sqlite-vec 本地语义检索
- 思维图谱可视化（按主题着色）
- 首页双列表（最近 + 对话最多）
- 关联想法自动发现

**🔒 隐私优先**
- 默认 100% 本地 SQLite
- BYO LLM Key + 预算硬上限
- 云同步明确可选（L2/L3）
- 端到端加密同步（L3 规划中）

</td>
</tr>
</table>

## 反馈渠道

- 🐛 Bug / 功能建议：[提交 Issue](https://github.com/Qc-riviere/EchoMind-releases/issues/new)
- 💬 微信交流群：（联系作者获取入群方式）
- 📧 邮件：见 GitHub profile

## FAQ

**Q：是开源软件吗？**
A：当前为内测阶段，源码未公开。本仓库仅托管 README、文档与发布包。计划未来视情况选择性开源（详见 [LICENSE](./LICENSE)）。

**Q：会上传我的数据到云端吗？**
A：默认不会。所有数据存在本机 SQLite。云同步是明确的可选项，开通时会有知情同意说明。

**Q：需要付费吗？**
A：本地版（L1 Core）永久免费。云端服务（L2 Bridge ¥99/年）和多设备同步（L3 Sync ¥199/年）为可选订阅，将在 Beta 公开发布后启用。

**Q：API Key 是怎么用的？**
A：所有 LLM 调用从你自己的 API Key 直接出，平台不中转。可选「通过云桥调用」模式由你显式开启，并设预算硬上限。

**Q：支持 Linux 吗？**
A：暂不分发 Linux 二进制；如有需求请提 Issue。

## 路线图

- ✅ v0.1 – v0.3.x — Alpha 内测（当前）：核心速记 + 微信桥 + AI 加工 + 本地检索 + UX 打磨
- ⏳ v0.4 — Beta 公开：Apple 签名、Landing 页、L2 ¥99 订阅开通
- ⏳ v0.5 — L3 Sync：多端端到端加密同步
- ⏳ v1.0 — 英文国际化

## 致谢

EchoMind 站在以下开源项目肩膀上：[Tauri](https://tauri.app) · [React](https://react.dev) · [SQLite](https://sqlite.org) · [sqlite-vec](https://github.com/asg017/sqlite-vec) · [腾讯 OpenClaw](https://github.com/tencent-weixin/openclaw-weixin)

---

<div align="center">

**EchoMind** © 2026 Qc-riviere · All rights reserved · [LICENSE](./LICENSE)

</div>
