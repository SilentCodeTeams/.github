# SilentCodeTeams

**Part of [SilentStudio](https://github.com/Silent-Studio-CN)**

Open-source network protocol tooling, developer tools and authorized security
testing infrastructure.

SilentCodeTeams 是 SilentStudio 旗下的开源工程小组，专注于网络协议分析、
开发者工具与授权安全测试基础设施。

## 我们在做什么

- **NetTool ζ**：Rust 实现的网络协议分析与授权安全测试核心。协议注册表、
  透明代理、真实 pcap、跨平台 CLI，后续接入 Qt 客户端与独立后台 daemon。
- **跨平台**：macOS、Windows x64/ARM64、Linux。
- **可扩展**：协议 dissector、C ABI 插件、可独立部署的 helper。
- **可验证**：单元测试、三平台 CI、真实 pcap 输出。

## 项目

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| NetTool ζ | Rust 网络协议分析与授权安全测试核心 | Private preview |
| More tools | 开发者工具与协议实验 | 规划中 |

## 工程原则

- Rust 优先；C 只用于操作系统薄垫片。
- 核心依赖少、可离线构建，解析器可单独测试与 fuzz。
- UI 与后台分离：Qt 客户端只通过本地 API 通信，崩溃不影响后台。
- 多版本协议：TLS/SSL、HTTP、DNS、QUIC、WebSocket、Minecraft。

## 安全与合规

- 只用于自有网络或获得书面授权的测试。
- 不提供隐蔽、规避监控或未经授权的远程控制功能。
- 默认本地监听、显式授权、审计日志、可恢复。
- 安全问题请按各仓库的 SECURITY.md 私下报告。

## 链接

- SilentStudio: https://github.com/Silent-Studio-CN
- 组织主页: https://github.com/SilentCodeTeams

---

**English**: SilentCodeTeams is the open-source engineering group of
SilentStudio, building network protocol tooling and authorized security
testing infrastructure. Rust-first, cross-platform, auditable by design.
