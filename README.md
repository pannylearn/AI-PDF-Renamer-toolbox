# AI PDF Renamer Toolbox

AI PDF Renamer Toolbox 是一个基于人工智能的PDF文件重命名工具，能够自动分析PDF内容并根据标题、作者和年份智能重命名文件。

本项目基于 [Web3NL/AI-PDF-Renamer](https://github.com/Web3NL/AI-PDF-Renamer) 开发，增加了对GLM-4V系列模型的支持和图形界面工具箱功能。

## 功能特点

- 🧠 支持多种AI模型：GLM-4V-Flash（推荐）、GLM-4V-Plus、Gemini Flash、Gemini Pro
- 🖼️ 通过分析PDF封面自动提取标题、作者和年份信息
- 📁 批量处理整个文件夹中的PDF文件
- 🖱️ 图形界面工具箱，简单易用
- ⚙️ 可配置分析页数以平衡准确性和成本

## 下载独立应用程序

### macOS版本

1. 下载最新的 `AI-PDF-Renamer-Toolbox-MacOS.zip` 文件
2. 解压缩下载的文件
3. 双击 `AI-PDF-Renamer-Toolbox.app` 启动应用程序

### 源代码版本

如果您希望从源代码运行或进行开发，请查看源代码分支。

## 配置API密钥

首次使用时需要配置API密钥：

1. 获取ZhipuAI API密钥：
   - 访问 https://open.bigmodel.cn/
   - 注册账号并获取API密钥

2. 在工具箱界面中：
   - 在API Key输入框中粘贴您的密钥
   - 选择"glm-4v-flash"模型（推荐）

## 使用方法

### 图形界面模式（推荐）

双击应用程序图标启动工具箱：
1. 输入您的API密钥（支持ZhipuAI或Google Gemini）
2. 选择包含PDF文件的文件夹
3. 选择输出文件夹
4. 点击"开始处理"

### 命令行模式

如果您更喜欢命令行方式，也可以在终端中运行：

```bash
# 进入应用程序包内部
cd AI-PDF-Renamer-Toolbox.app/Contents/MacOS/

# 运行应用程序
./AI-PDF-Renamer-Toolbox
```

## 系统要求

- macOS 10.15 或更高版本
- 网络连接（用于AI API调用）

## 致谢

本项目基于 [Web3NL/AI-PDF-Renamer](https://github.com/Web3NL/AI-PDF-Renamer) 开发，在此感谢原作者的贡献。

## 许可证

本项目采用MIT许可证 - 查看 [LICENSE](LICENSE) 文件了解详情