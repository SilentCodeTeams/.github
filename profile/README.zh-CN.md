# SilentCodeTeams

**SilentStudio 旗下开源工程组**

[English](README.md) | 简体中文

SilentCodeTeams 是 SilentStudio 旗下的开源工程小组，专注于网络协议工具、
开发者工具与授权安全测试基础设施。

## 我们在做什么

- **NetTool ζ**：Rust 实现的网络协议分析与授权安全测试核心。协议注册表、
  透明代理、真实 pcap、跨平台 CLI，以及独立的 daemon/UI 进程边界。
- 跨平台：macOS、Windows x64/ARM64、Linux。
- 可扩展：协议 dissector、C ABI 插件、独立 helper。
- 可验证：单元测试、三平台 CI、真实 pcap 输出。

## 项目

| 项目 | 说明 | 状态 |
| --- | --- | --- |
| NetTool ζ | Rust 网络协议分析与授权安全测试核心 | 公开 |

## 工程原则

- Rust 优先；C 只用于操作系统薄垫片。
- 依赖少、可离线构建，解析器可单独测试与 fuzz。
- UI 与后台分离：UI 崩溃不会影响后台。
- 多版本协议：TLS/SSL、HTTP、DNS、QUIC、WebSocket、Minecraft。

## 安全与合规

- 仅用于自有系统或获得书面授权的测试。
- 不提供隐蔽、规避监控或未经授权的远程控制能力。
- 默认本地监听、显式授权、审计日志、可恢复。
- 安全问题请按各仓库的 SECURITY.md 私下报告。

## 链接

- NetTool ζ: https://github.com/SilentCodeTeams/nettool
- SilentStudio: https://github.com/Silent-Studio-CN
- 组织主页: https://github.com/SilentCodeTeams
