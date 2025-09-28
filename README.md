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

1. 访问 [Releases](https://github.com/pannylearn/AI-PDF-Renamer-toolbox/releases) 页面
2. 下载最新的 `AI-PDF-Renamer-Toolbox-MacOS.zip` 文件
3. 解压缩下载的文件
4. 双击 `AI-PDF-Renamer-Toolbox.app` 启动应用程序

### 源代码版本

如果您希望从源代码运行或进行开发，可以克隆此仓库并按照以下步骤操作：

```bash
# 克隆仓库
git clone https://github.com/pannylearn/AI-PDF-Renamer-toolbox.git
cd AI-PDF-Renamer-toolbox

# 安装依赖
pip install -r requirements.txt

# 安装系统依赖
# macOS: brew install poppler
# Ubuntu/Debian: sudo apt-get install poppler-utils

# 启动工具箱
python toolbox.py
```

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

双击应用程序图标或运行：

```bash
python toolbox.py
```

在图形界面中：
1. 输入您的API密钥（支持ZhipuAI或Google Gemini）
2. 选择包含PDF文件的文件夹
3. 选择输出文件夹
4. 点击"开始处理"

### 命令行模式

```bash
# 基本用法
python src/main.py /path/to/input/pdfs /path/to/output

# 使用特定模型
python src/main.py /input /output --model glm-4v-flash

# 只分析前3页以提高准确性
python src/main.py /input /output --max-pages 3

# 仅提取元数据，不复制文件
python src/main.py /input /output --no-copy
```

## 系统要求

### 独立应用程序
- macOS 10.15 或更高版本

### 源代码版本
- Python 3.7+
- macOS、Windows 或 Linux 操作系统
- poppler-utils (用于PDF处理)

## 致谢

本项目基于 [Web3NL/AI-PDF-Renamer](https://github.com/Web3NL/AI-PDF-Renamer) 开发，在此感谢原作者的贡献。

## 许可证

本项目采用MIT许可证 - 查看 [LICENSE](LICENSE) 文件了解详情