# AlertDog Docs

<div align="center">

[![Mintlify](https://img.shields.io/badge/Built%20with-Mintlify-brightgreen)](https://mintlify.com)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Languages](https://img.shields.io/badge/languages-中文%20%7C%20English-orange)](docs.json)

**WEB3 链上监控报警系统的完整技术文档**

[在线文档](https://docs.alertdog.io) | [AlertDog 官网](https://alertdog.io) | [问题反馈](https://github.com/alertdogio/docs/issues)

</div>

---

## 项目简介

本仓库是 **AlertDog** 的官方文档站点，提供完整的产品使用指南、API 文档、案例教程和常见问题解答。

AlertDog 是一款专业的 WEB3 链上监控报警系统，支持 EVM、Solana、Bitcoin、SUI 等多条主流区块链的实时监控。

---

## 快速开始

### 环境要求

- Node.js 20+
- npm 或 yarn

### 本地开发

1. **克隆仓库**

```bash
git clone https://github.com/alertdogio/docs.git alertdog-docs
cd alertdog-docs
```

2. **安装 Mintlify CLI**

```bash
npm i -g mint
```

3. **启动开发服务器**

```bash
mint dev
```

4. **访问预览**

打开浏览器访问 `http://localhost:3000`

### 常用命令

```bash
# 更新 Mintlify CLI 到最新版本
mint update

# 检查文档格式
mint validate

# 构建生产版本
mint build
```

---

## 更新指南

### 文档编写规范

我们遵循 [Mintlify 技术写作规范](https://mintlify.com/docs/content/text)，核心要求：

#### 1. 语言风格

- 使用第二人称（"您"、"You"）
- 使用主动语态
- 保持简洁明了
- 避免不必要的术语

#### 2. 内容组织

- 使用 `<Steps>` 组件展示流程
- 使用 `<Tip>`、`<Warning>`、`<Note>` 等标注重要信息
- 为所有图片添加描述性 alt 属性
- 使用清晰的标题和章节分隔

#### 3. SEO 优化

- 每个文档必须有 `title` 和 `description`
- 图片文件名使用描述性命名（如 `wallet-login-select.png`）
- 内部链接使用相对路径
- 标题包含关键词

#### 4. Snippets 使用

对于重复内容，使用 Snippets 避免代码重复：

```mdx
<Steps>
<Snippet file="zh/step-sign-in.mdx" />
<Snippet file="zh/step-add-notification.mdx" />

<Step title="你的自定义步骤">
  <!-- 自定义内容 -->
</Step>

<Snippet file="zh/step-receive-alert.mdx" />
</Steps>
```

详细说明请参考 [`snippets/README.mdx`](snippets/README.mdx)

## 配置说明

### docs.json

`docs.json` 是文档的核心配置文件，包含：

- **导航结构**: 定义文档目录树
- **双语配置**: 中英文切换
- **主题设置**: 颜色、Logo、favicon
- **导航栏**: 外部链接和按钮

关键配置项：

```json
{
  "name": "AlertDog Docs",
  "theme": "palm",
  "colors": {
    "primary": "#ea9148",
    "light": "#ea9148",
    "dark": "#ea9148"
  },
  "navigation": {
    "languages": [
      {
        "language": "zh",
        "default": true,
        "tabs": [
          /* ... */
        ]
      },
      {
        "language": "en",
        "tabs": [
          /* ... */
        ]
      }
    ]
  }
}
```

完整配置参考 [Mintlify docs.json Schema](https://mintlify.com/docs.json)

---

## 部署

### 自动部署

本项目通过 GitHub App 自动部署到 Mintlify：

1. 推送到 `main` 分支
2. GitHub App 自动触发构建
3. 几分钟后即可在 [docs.alertdog.io](https://docs.alertdog.io) 查看

### 手动部署

如需手动部署，请参考 [Mintlify 部署指南](https://mintlify.com/docs/settings/deployment)

---

## 社区与支持

- **Twitter**: [@alertdogio](https://x.com/alertdogio)
- **Telegram**: [AlertDog Community](https://t.me/alertdog)
- **问题反馈**: [GitHub Issues](https://github.com/alertdogio/docs/issues)

---

## 致谢

- [Mintlify](https://mintlify.com) - 提供优秀的文档框架
- 所有为本项目贡献内容的开发者
- AlertDog 用户社区的反馈和建议

---

<div align="center">

**[AlertDog](https://alertdog.io)** - 您的 WEB3 链上监控专家

Made with love by [MCT Team](https://mct.xyz)

</div>
