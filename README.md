# 多模型AI聊天助手

一个简单的网页应用，可以通过 OpenRouter.ai API 调用多种大语言模型，支持在对话过程中自由切换不同模型。

## 功能特点

- **多模型支持**: 支持 Claude 3.5 Sonnet、GPT-4o、GPT-4o Mini、Gemini Pro 1.5、Llama 3.1 70B、Mixtral 8x7B 等主流模型
- **实时切换**: 在对话过程中可以随时切换模型
- **对话历史**: 自动保存对话历史，支持上下文连续对话
- **本地存储**: 使用浏览器本地存储保存 API 密钥和对话记录
- **响应式设计**: 支持桌面和移动设备
- **简洁界面**: 现代化的聊天界面，易于使用
- **错误处理**: 完善的错误提示和处理机制

## 使用方法

1. **获取 API 密钥**
   - 访问 [OpenRouter.ai](https://openrouter.ai/) 注册账户
   - 在账户设置中生成 API 密钥

2. **打开应用**
   - 直接在浏览器中打开 `index.html` 文件
   - 或者使用本地服务器运行

3. **配置和使用**
   - 在页面顶部输入您的 OpenRouter API 密钥
   - 选择想要使用的模型

 # 🤖 AI Chat Interface

多模型AI聊天界面，支持角色定制和智能搜索

## ✨ 功能特性

- 🤖 **多模型支持**: Claude 3.5 Sonnet, GPT-4o, Gemini Pro等
- 🎭 **角色定制**: 5种预设角色 + 自定义AI人格
- 🔍 **智能搜索**: DuckDuckGo实时搜索增强
- ✏️ **消息编辑**: 编辑历史消息并重新生成回答
- 💬 **对话管理**: 智能上下文管理和备忘录
- 💾 **数据持久**: 本地存储所有设置和对话

## 🚀 GitHub部署方案

### 方案1: GitHub Pages (静态版本)
1. 创建GitHub仓库
2. 上传所有文件
3. Settings → Pages → Deploy from branch → main
4. 访问: `https://用户名.github.io/仓库名`

**注意**: GitHub Pages仅支持静态文件，后端API功能需配合其他服务

### 方案2: GitHub + Netlify (推荐)
1. 上传代码到GitHub
2. 连接Netlify到GitHub仓库
3. 自动部署，支持完整功能

### 方案3: GitHub + Vercel
1. 上传代码到GitHub  
2. 导入Vercel项目
3. 自动部署

## 📁 文件结构

```
├── index.html              # 主应用文件
├── server.js               # 本地开发服务器
├── package.json            # 项目配置
├── netlify.toml           # Netlify部署配置
├── netlify/functions/     # 无服务器函数
│   ├── chat.js           # OpenRouter API代理
│   └── search.js         # DuckDuckGo搜索代理
└── .gitignore            # Git忽略文件
```

## 🔧 本地运行

```bash
node server.js
# 访问 http://localhost:3000
```

## 🌐 在线演示

部署后即可在线使用，需要OpenRouter API密钥

## 📄 许可证

MIT License

## 支持的模型

- **Claude 3.5 Sonnet** - Anthropic 最新模型
- **GPT-4o** - OpenAI 最新多模态模型  
- **GPT-4o Mini** - OpenAI 轻量级模型
- **Gemini Pro 1.5** - Google 大语言模型
- **Llama 3.1 70B** - Meta 开源模型
- **Mixtral 8x7B** - Mistral AI 混合专家模型

## 注意事项

- 需要有效的 OpenRouter API 密钥才能使用
- API 调用会产生费用，请注意使用量
- 对话历史保存在本地浏览器中，清除浏览器数据会丢失历史记录
- 建议在稳定的网络环境下使用

## 浏览器兼容性

支持所有现代浏览器，包括：
- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+
