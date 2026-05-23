<div align="center">

# 星云AI Ultra

**开源免费的 AI 聊天工具，支持多个大模型，开箱即用**

[在线体验](https://yyh-0428.github.io/nebula-ai-pro/) · [GitHub](https://github.com/yyh-0428/nebula-ai-pro) · [反馈建议](https://github.com/yyh-0428/nebula-ai-pro/issues)

![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-在线可用-blue?style=flat-square&logo=github)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)
![Stars](https://img.shields.io/github/stars/yyh-0428/nebula-ai-pro?style=flat-square)
![Forks](https://img.shields.io/github/forks/yyh-0428/nebula-ai-pro?style=flat-square)

</div>

---

## 功能亮点

| 功能 | 说明 |
|------|------|
| **多模型支持** | DeepSeek、GPT-4o、Claude、通义千问、Ollama 本地模型等 |
| **对话分支** | 编辑任意消息，从任意节点重新生成，保留所有对话路径 |
| **可视化模式** | 对话树状可视化展示，一键切换分支 |
| **深度思考** | 支持 DeepSeek-R1 等推理模型的思维链展示 |
| **联网搜索** | 对话前自动搜索互联网，获取最新信息 |
| **全局记忆** | 记住你的偏好和上下文，AI 越用越懂你 |
| **文件上传** | 拖拽/粘贴图片直接发送 |
| **云端同步** | 注册账号后多设备同步对话记录 |
| **深色模式** | 护眼深色主题，一键切换 |
| **快捷键** | 丰富的键盘快捷键，高效操作 |
| **零门槛** | 打开网页即用，无需下载安装 |

## 快速开始

### 1. 打开应用

直接访问：**https://yyh-0428.github.io/nebula-ai-pro/**

### 2. 配置 API Key

点击右上角 ⚙️ 设置图标，选择你要使用的模型：

| 模型 | API 地址 | 说明 |
|------|----------|------|
| **DeepSeek** | `https://api.deepseek.com` | 国产高性价比，推荐入门 |
| **GPT-4o** | `https://api.openai.com/v1` | OpenAI 最新模型 |
| **Claude** | `https://api.anthropic.com/v1` | Anthropic 出品 |
| **通义千问** | `https://dashscope.aliyuncs.com/compatible-mode/v1` | 阿里云大模型 |
| **Ollama** | `http://localhost:11434/v1` | 本地部署，免费无限 |

填入对应的 API Key，点击保存即可开始对话。

### 3. 开始聊天

- `Enter` 发送消息
- `Shift+Enter` 换行
- `Ctrl+Shift+N` 新建对话
- `Ctrl+/` 查看全部快捷键

## 功能演示

### 对话分支

编辑任意一条消息，自动创建新分支，保留原对话路径。点击右上角 🔀 分支图标查看所有分支。

### 可视化模式

点击右上角 🖼 可视化图标，将对话以树状图展示，点击节点即可切换分支。

### 深度思考

开启深度思考模式后，AI 会先展示推理过程，再给出最终答案。支持 DeepSeek-R1 等推理模型。

### 联网搜索

开启联网搜索后，AI 会在回答前自动搜索互联网，获取最新信息。

## 技术栈

- **前端**：原生 HTML/CSS/JavaScript，零框架依赖
- **渲染**：Marked.js（Markdown）+ Highlight.js（代码高亮）+ KaTeX（数学公式）
- **存储**：localStorage（本地）+ PocketBase（云端同步）
- **部署**：GitHub Pages，全球 CDN 加速

## 本地部署

如果你想自己部署或二次开发：

```bash
# 克隆仓库
git clone https://github.com/yyh-0428/nebula-ai-pro.git
cd nebula-ai-pro

# 直接用浏览器打开
open index.html

# 或者启动本地服务器
python3 -m http.server 8080
# 访问 http://localhost:8080
```

### 云端同步（可选）

```bash
# 安装 PocketBase
curl -L https://github.com/pocketbase/pocketbase/releases/download/v0.38.2/pocketbase_0.38.2_darwin_arm64.zip -o pb.zip
unzip pb.zip

# 启动
./pocketbase serve

# 访问管理后台 http://127.0.0.1:8090/_/ 创建账号
```

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Enter` | 发送消息 |
| `Shift+Enter` | 换行 |
| `Ctrl+Shift+N` | 新建对话 |
| `Ctrl+Shift+X` | 清空对话 |
| `Ctrl+Shift+E` | 导出对话 |
| `Ctrl+,` | 打开设置 |
| `Ctrl+K` | 切换联网搜索 |
| `Ctrl+/` | 显示快捷键帮助 |
| `Esc` | 停止生成 / 关闭弹窗 |

## 为什么选择星云AI？

| 对比项 | 星云AI Ultra | 其他工具 |
|--------|-------------|----------|
| **费用** | 完全免费，只付 API 费用 | 部分收费 |
| **隐私** | 数据存本地/自建服务器 | 数据存第三方 |
| **模型** | 自由切换任意模型 | 绑定单一模型 |
| **开源** | 完全开源，可自由修改 | 闭源 |
| **部署** | 一行命令，打开即用 | 需要复杂配置 |

## 贡献

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建功能分支：`git checkout -b feature/amazing-feature`
3. 提交更改：`git commit -m 'Add amazing feature'`
4. 推送分支：`git push origin feature/amazing-feature`
5. 提交 Pull Request

## 许可证

MIT License - 自由使用、修改和分发。

## 支持

如果这个项目对你有帮助，请给一个 ⭐ Star 支持一下！

有问题或建议？[提交 Issue](https://github.com/yyh-0428/nebula-ai-pro/issues)

---

<div align="center">

**[立即体验](https://yyh-0428.github.io/nebula-ai-pro/)** · **[GitHub](https://github.com/yyh-0428/nebula-ai-pro)**

Made with ❤️ by [yyh-0428](https://github.com/yyh-0428)

</div>
