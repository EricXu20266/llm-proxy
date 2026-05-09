# LLMProxy

> Codex Desktop & Claude CLI → DeepSeek 本地协议翻译代理 | Agent Protocol Translation Proxy

LLMProxy 是一个 Windows 桌面应用，在本地 127.0.0.1 启动协议翻译代理服务，让 Codex Desktop（Responses API）和 Claude CLI（Anthropic Messages API）无缝接入 DeepSeek 等 OpenAI 兼容的三方大模型供应商。

---

## 快速开始

1. 从 [Releases](https://github.com/) 下载最新 `LLMProxy x.x.x.msi`
2. 安装并启动
3. 点击右上角 **启动服务**
4. 配置 Provider → API Key → Model Mapping
5. 在 Settings 中复制 Codex Desktop 配置，粘贴到 Codex 配置文件

---

## 功能

- **协议翻译**：Responses API / Anthropic Messages → Chat Completions
- **管理面板**：可视化管理 Provider、API Key、Model Mapping
- **实时控制台**：SSE 流式日志，暂停/下载
- **中英文切换**：界面完整 i18n 支持
- **端口可调**：默认 8000，可在 Settings 中修改
- **配置导入/导出**：一键迁移配置
- **请求日志**：完整的代理请求历史

---

## 验证

```
SHA256: 94833a63b865522ad3cd6d93aa4a76cc46b105b7386f8aa44948a872f9635374
```

```bash
certutil -hashfile "LLMProxy 0.5.0.msi" SHA256
```

---

## 作者

**二班的Eric Xu**

## 协议

MIT License
