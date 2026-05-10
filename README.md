# LLMProxy

> Codex Desktop & Claude CLI → DeepSeek 本地协议翻译代理 | Agent Protocol Translation Proxy

LLMProxy 是一个运行在 Windows 以及 Mac OS 上的桌面应用，在本地 127.0.0.1 启动协议翻译代理服务，让 Codex Desktop（Responses API）和 Claude Cwork（Anthropic Messages API）无缝接入 DeepSeek 等 OpenAI 兼容的三方大模型供应商。

此代理仅在两个智能体的桌面版测试成功，CLI上未进行测试。

---

## 快速开始

1. 从 [Releases](https://github.com/) 下载最新 `LLMProxy x.x.x.msi`
2. 安装并启动
3. 点击右上角 **启动服务**
4. 配置 Provider → API Key → Model Mapping
5. 在 Settings 中复制 Codex Desktop 配置，粘贴到 Codex 配置文件
6. Claude Cwork先尝试在开发者模式下配置第三方llm的方式直接接入3方模型，如果不行，再尝试使用代理（当然同样是需要在三方模式下，填入代理地址）

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
### Apple Mac OS version "LLMProxy-0.5.0.dmg" SHA256
```
SHA256: 77f3a49a8a784d5529769dec4ad0cd70a6697884428616fa36b90112a0fad3e7
```

```bash
shasum -a 256 "LLMProxy-0.5.0.dmg"
```

### Microsoft Windows version "LLMProxy 0.5.0.msi" SHA256
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
