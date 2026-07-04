<div align="center">

# AVL Code

**国产 AI 智能编程与安全分析桌面助手**
**AI-native coding & security-analysis desktop assistant**

[![Release](https://img.shields.io/badge/release-alpha%20%C2%B7%20rolling-blue)](https://www.avlcode.cn/changelog/)
[![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey)](https://www.avlcode.cn/#download)
[![Website](https://img.shields.io/badge/website-avlcode.cn-0a7)](https://www.avlcode.cn/)
[![License](https://img.shields.io/badge/license-Proprietary-red)](LICENSE)

**简体中文** · [English](#english) · [繁體中文](#繁體中文)

</div>

> [!NOTE]
> **本仓库仅用于发布记录与社区问题反馈追踪,不包含产品源代码。**
> This repository is for **release records and community issue tracking only** — it does **not** contain product source code.
> 本倉庫僅用於發佈記錄與社群問題回饋追蹤,不包含產品原始碼。

---

## 最近发布 / Recent Releases / 最近發佈

> 仅展示最近 3 天的滚动发布,同一天若有多个版本则每个版本各占一行;完整记录见[发布日志](https://www.avlcode.cn/changelog/)。
> Showing the last 3 days only — one row per version (multiple rows if a day has several); see the full [changelog](https://www.avlcode.cn/changelog/).

| 日期 Date | 版本 Version | 说明 Summary |
| --- | --- | --- |
| 2026-07-04 | `v0.7.4-alpha.1909` | 升级弹窗说明与发布说明一致,账号用量对齐服务端(可用点数 / 滑动窗口恢复),VirusTotal AI 支持独立接入点;修复最大化时遮罩与圆角错位。 |
| 2026-07-03 | `v0.7.3-alpha.1534` | 新增 VirusTotal / Google Threat Intelligence 全量工具组(`vt.*`,查询 / 提交 / 下载 / 狩猎,分级门控);安全设置重构,检测能力与哨兵拦截解耦。 |
| 2026-07-02 | `v0.7.2-alpha.1851` | IOC 提取(`sec.ioc_extract`)增强:还原 defang 输入、有效性校验,新增 CVE / 注册表 / MAC / SHA-512 / 钱包地址等类型,附频次与分页。 |
| 2026-07-02 | `v0.7.2-alpha.1223` | 全库代码问答(`code.ask` / RAG)检索质量提升:结构感知智能重排,增量刷新作用域修正;修复导入 / 重建会话误报「已存在」。 |
| 2026-07-02 | `v0.7.2-alpha.0917` | 会话导出脱敏递归下钻嵌套 JSON,覆盖工具调用参数与结果中的敏感信息。 |

---

## 简体中文

### 什么是 AVL Code

AVL Code 是[安天(Antiy)](https://www.antiy.cn/)澜砥团队推出的国产 AI 智能编程与安全分析桌面助手,Windows / macOS / Linux 全平台原生分发。它把对话式 AI 与工程师真实工作台合二为一:**读写代码、执行命令、研判恶意样本**,审批与进度通过微信 / 飞书 / 钉钉随行到手机。搭载澜砥威胁检测分析(人工智能)垂直大模型与安天 AVL 安全引擎。

### 核心特性

- **同类智能体编程工具** — 与 Claude Code、OpenAI Codex 同类的 agentic coding 工具,国产自主可控的替代选择。
- **生态平滑迁移** — 兼容 Claude Code 生态习惯:`AGENTS.md` / `CLAUDE.md` 项目指令自动注入,标准 subagent_type 子代理别名,既有工作流平滑迁移。
- **内置安全基因** — 面向二进制的只读分析工具组(哈希 / 熵、IOC 抽取、PE/ELF/Mach-O 解析、反汇编、C/Java 伪代码反编译、YARA 规则匹配);`samples/` 样本区强制禁用执行类工具。
- **安全强化 · 自主可控** — 本地凭据国密 SM4-GCM 加密,技能包 SM2/SM3 国密签名,会话 100% 本地保存;企业版支持全栈私有化部署与等保适配。
- **五种工作模式** — 自动 / 筹划 / 准备 / 执行 / 评估,支持长程任务,不止步于编程。
- **灵活模型接入** — AVL Delta 高效协议接澜砥模型;OpenAI / Anthropic 兼容协议接自有或第三方模型。

### 下载与文档

| 资源 | 链接 |
| --- | --- |
| 全平台下载 | <https://www.avlcode.cn/#download> |
| 快速上手指南 | <https://www.avlcode.cn/docs/quick-start/> |
| 用户手册 | <https://www.avlcode.cn/docs/user-manual/> |
| 参考手册 | <https://www.avlcode.cn/docs/reference/> |
| 发布日志 | <https://www.avlcode.cn/changelog/> |
| 实战案例 | <https://www.avlcode.cn/cases/> |

支持平台:Windows x64 · macOS(Universal 与 Apple 芯片)· Linux(通用、AppImage、Snap、WebKit 4.1)。

### 发布产物声明

- AVL Code 当前处于**内测(Alpha)阶段**,所有发布产物均以**「按现状(AS IS)/ 按可用(AS AVAILABLE)」**提供,功能与可用性可能随时调整或中止。
- 请仅从**官方渠道**([avlcode.cn](https://www.avlcode.cn/#download))或本仓库 Releases 获取安装包,并核对完整性,以防被篡改或植入恶意内容。
- 发布渠道仅保留**最近约一个月**的滚动版本;历史版本可能被移除。
- 所有发布产物的使用受 [LICENSE](LICENSE) 与《[AVL Code 使用许可协议](https://www.avlcode.cn/legal/terms/)》约束,本仓库不授予任何开源许可。

### 反馈与问题

发现 Bug、想提需求或参与讨论,欢迎通过本仓库的 **[Issues](../../issues)** 提交。提交前请:

1. 先**搜索**已有 Issue,避免重复;
2. 注明 **AVL Code 版本号**、**操作系统**与复现步骤;
3. 涉及安全分析样本时,**请勿上传真实恶意样本**,改用哈希值或脱敏描述。

### 出品方

[安天科技集团(Antiy)· 澜砥团队](https://www.antiy.cn/)
服务备案号:Heilongjiang-Landi-20241217S0001 · 算法备案号:网信算备230109026778501240017号

---

## English

### What is AVL Code

AVL Code is an AI-native coding and security-analysis desktop assistant from the **Landi (澜砥) team at [Antiy](https://www.antiy.cn/)**, distributed natively across Windows / macOS / Linux. It merges conversational AI with an engineer's real workbench — **reading and writing code, running commands, and triaging malware samples** — with approvals and progress following you to your phone via WeChat / Feishu / DingTalk. Powered by Landi's threat-detection vertical LLM and the Antiy AVL security engine.

### Highlights

- **Agentic coding tool** — In the same class as Claude Code and OpenAI Codex, built as a domestic, self-controlled alternative.
- **Smooth ecosystem migration** — Compatible with Claude Code conventions: automatic `AGENTS.md` / `CLAUDE.md` project-instruction injection and standard `subagent_type` aliases, so existing workflows carry over.
- **Security in its DNA** — A read-only binary analysis toolset (hash/entropy, IOC extraction, PE/ELF/Mach-O parsing, disassembly, C/Java pseudocode decompilation, YARA matching); execution tools are force-disabled inside the `samples/` area.
- **Hardened & self-controlled** — Local credentials encrypted with SM4-GCM (Chinese national crypto), skill packages signed with SM2/SM3, sessions stored 100% locally; the enterprise edition supports full private deployment and compliance adaptation.
- **Five working modes** — Auto / Plan / Prepare / Execute / Evaluate, with support for long-horizon tasks beyond coding.
- **Flexible model access** — AVL Delta protocol for Landi models; OpenAI / Anthropic-compatible protocols for your own or third-party models.

### Download & Docs

| Resource | Link |
| --- | --- |
| Download (all platforms) | <https://www.avlcode.cn/#download> |
| Quick Start | <https://www.avlcode.cn/docs/quick-start/> |
| User Manual | <https://www.avlcode.cn/docs/user-manual/> |
| Reference | <https://www.avlcode.cn/docs/reference/> |
| Changelog | <https://www.avlcode.cn/changelog/> |
| Case Studies | <https://www.avlcode.cn/cases/> |

Supported platforms: Windows x64 · macOS (Universal & Apple Silicon) · Linux (generic, AppImage, Snap, WebKit 4.1).

### Release Artifacts Notice

- AVL Code is currently in **Alpha (beta) testing**. All release artifacts are provided **"AS IS" / "AS AVAILABLE"**; features and availability may change or be suspended at any time.
- Obtain installers only from **official channels** ([avlcode.cn](https://www.avlcode.cn/#download)) or this repository's Releases, and verify their integrity to guard against tampering or malicious modification.
- The release channel keeps only the **most recent ~1 month** of rolling builds; older versions may be removed.
- Use of all release artifacts is governed by [LICENSE](LICENSE) and the [AVL Code EULA](https://www.avlcode.cn/legal/terms/). This repository grants no open-source license.

### Feedback & Issues

Found a bug, have a feature request, or want to join the discussion? Please open an **[Issue](../../issues)** in this repository. Before submitting:

1. **Search** existing issues to avoid duplicates;
2. Include your **AVL Code version**, **operating system**, and reproduction steps;
3. For security-analysis cases, **do not upload real malware samples** — use hashes or redacted descriptions instead.

### Publisher

[Antiy Technology Group · Landi Team](https://www.antiy.cn/)
Service filing: Heilongjiang-Landi-20241217S0001 · Algorithm filing: 网信算备230109026778501240017号

---

## 繁體中文

### 什麼是 AVL Code

AVL Code 是[安天(Antiy)](https://www.antiy.cn/)澜砥團隊推出的 AI 智慧程式設計與安全分析桌面助手,Windows / macOS / Linux 全平台原生分發。它將對話式 AI 與工程師真實工作檯合而為一:**讀寫程式碼、執行命令、研判惡意樣本**,審批與進度透過微信 / 飛書 / 釘釘隨行到手機。搭載澜砥威脅偵測分析(人工智慧)垂直大模型與安天 AVL 安全引擎。

### 核心特性

- **同類智慧體程式設計工具** — 與 Claude Code、OpenAI Codex 同類的 agentic coding 工具,自主可控的替代選擇。
- **生態平滑遷移** — 相容 Claude Code 生態習慣:`AGENTS.md` / `CLAUDE.md` 專案指令自動注入,標準 subagent_type 子代理別名,既有工作流平滑遷移。
- **內建安全基因** — 面向二進位的唯讀分析工具組(雜湊 / 熵、IOC 抽取、PE/ELF/Mach-O 解析、反組譯、C/Java 偽程式碼反編譯、YARA 規則比對);`samples/` 樣本區強制停用執行類工具。
- **安全強化 · 自主可控** — 本地憑證國密 SM4-GCM 加密,技能包 SM2/SM3 國密簽章,工作階段 100% 本地保存;企業版支援全棧私有化部署與等保適配。
- **五種工作模式** — 自動 / 籌劃 / 準備 / 執行 / 評估,支援長程任務,不止步於程式設計。
- **靈活模型接入** — AVL Delta 高效協定接澜砥模型;OpenAI / Anthropic 相容協定接自有或第三方模型。

### 下載與文件

| 資源 | 連結 |
| --- | --- |
| 全平台下載 | <https://www.avlcode.cn/#download> |
| 快速上手指南 | <https://www.avlcode.cn/docs/quick-start/> |
| 使用者手冊 | <https://www.avlcode.cn/docs/user-manual/> |
| 參考手冊 | <https://www.avlcode.cn/docs/reference/> |
| 發佈日誌 | <https://www.avlcode.cn/changelog/> |
| 實戰案例 | <https://www.avlcode.cn/cases/> |

支援平台:Windows x64 · macOS(Universal 與 Apple 晶片)· Linux(通用、AppImage、Snap、WebKit 4.1)。

### 發佈產物聲明

- AVL Code 目前處於**內測(Alpha)階段**,所有發佈產物均以**「按現狀(AS IS)/ 按可用(AS AVAILABLE)」**提供,功能與可用性可能隨時調整或中止。
- 請僅從**官方渠道**([avlcode.cn](https://www.avlcode.cn/#download))或本倉庫 Releases 取得安裝包,並核對完整性,以防遭篡改或植入惡意內容。
- 發佈渠道僅保留**最近約一個月**的滾動版本;歷史版本可能被移除。
- 所有發佈產物的使用受 [LICENSE](LICENSE) 與《[AVL Code 使用許可協議](https://www.avlcode.cn/legal/terms/)》約束,本倉庫不授予任何開源授權。

### 回饋與問題

發現 Bug、想提需求或參與討論,歡迎透過本倉庫的 **[Issues](../../issues)** 提交。提交前請:

1. 先**搜尋**既有 Issue,避免重複;
2. 註明 **AVL Code 版本號**、**作業系統**與重現步驟;
3. 涉及安全分析樣本時,**請勿上傳真實惡意樣本**,改用雜湊值或去敏描述。

### 出品方

[安天科技集團(Antiy)· 澜砥團隊](https://www.antiy.cn/)
服務備案號:Heilongjiang-Landi-20241217S0001 · 演算法備案號:網信算備230109026778501240017號

---

## 学术引用 / Citation / 學術引用

如果 AVL Code 对您的研究或工作有所帮助,欢迎引用本项目。
If AVL Code helps your research or work, please consider citing it.
若 AVL Code 對您的研究或工作有所幫助,歡迎引用本專案。

```bibtex
@software{avlcode,
  title  = {AVL Code: An AI-native Coding and Security-analysis Desktop Assistant},
  author = {{Antiy Technology Group} and {Landi Team}},
  year   = {2026},
  url    = {https://www.avlcode.cn/},
  note   = {Alpha release}
}
```

---

<div align="center">

### ⭐ 欢迎 Star & Watch / Star & Watch Us / 歡迎 Star & Watch

如果您喜欢 AVL Code,欢迎点亮 **Star** 支持我们,并 **Watch** 本仓库以第一时间获取发布更新与公告。
If you like AVL Code, please give us a **Star** and **Watch** this repository to stay up to date with releases and announcements.
如果您喜歡 AVL Code,歡迎點亮 **Star** 支持我們,並 **Watch** 本倉庫以第一時間獲取發佈更新與公告。

<br>

<sub>© Antiy · Landi Team — AVL Code. 本仓库仅用于发布记录与社区反馈 / for releases & community feedback only.</sub>

</div>
