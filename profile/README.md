# SilentCodeTeams

**Part of [SilentStudio](https://github.com/Silent-Studio-CN)**

English | [简体中文](README.zh-CN.md)

SilentCodeTeams is the open-source engineering group of SilentStudio. We build
network protocol tooling, developer tools and authorized security testing
infrastructure.

## What we do

- **NetTool ζ**: Rust core for network protocol analysis and authorized
  security testing. Protocol registry, transparent proxy, real pcap,
  cross-platform CLI, and a separate daemon/UI boundary.
- Cross-platform: macOS, Windows x64/ARM64, Linux.
- Extensible: protocol dissectors, C ABI plugins, standalone helpers.
- Verifiable: unit tests, three-platform CI, real pcap output.

## Projects

| Project | Description | Status |
| --- | --- | --- |
| NetTool ζ | Rust network protocol analysis and authorized security testing core | Public |

## Principles

- Rust-first; C only for OS shims.
- Few dependencies, offline builds, parsers testable and fuzzable.
- UI and backend are separate processes; a UI crash does not stop the backend.
- Multi-version protocols: TLS/SSL, HTTP, DNS, QUIC, WebSocket, Minecraft.

## Security

- Use only on systems you own or are authorized to test.
- No stealth, evasion or unauthorized remote-control features.
- Local-only defaults, explicit authorization, audit logs, recovery.
- Report vulnerabilities per the repository SECURITY.md.

## Links

- NetTool ζ: https://github.com/SilentCodeTeams/nettool
- SilentStudio: https://github.com/Silent-Studio-CN
- Organization: https://github.com/SilentCodeTeams
