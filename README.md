# AI ChatBox - MFC桌面聊天助手

[![MFC](https://img.shields.io/badge/Framework-MFC-008080.svg)]()
[![C++](https://img.shields.io/badge/Language-C%2B%2B-00599C.svg)]()

## 📝 项目简介

AI ChatBox是一个基于MFC框架开发的本地AI聊天程序，集成了大型语言模型，支持多轮对话，对话记录保存，主题定制等功能。用户可以选择不同的本地模型，例如qwen、llama、deepseek等，进行对话。AI ChatBox完全离线运行，保护用户隐私。


## ▶  项目讲解

https://www.bilibili.com/video/BV1HbPkeZEQD

## ✨ 功能特性

- 💬 **多轮对话** - 支持上下文感知的连续对话
- 🧠 **本地推理** - 使用本地模型cpu推理
- 📚 **历史管理** - 对话记录保存与快速回溯
- 🎨 **主题定制** - 可调整字体/颜色/样式
- ⚡ **流式响应** - 实时生成Token显示
- 🛡️ **隐私保护** - 完全离线的本地化运行

## 🌟 效果展示

-  **可以选择不同的本地模型，例如qwen、llama、deepseek等**
![界面截图](image/设置.gif)
-  **可以查看本地保存的历史记录**
![界面截图](image/历史记录.gif)
-  **开启新聊天后，可以实时查看AI的回复**
![界面截图](image/新聊天.gif)

## 🚀 快速使用

1. 下载Release并解压缩到本地目录
2. 下载[llama.cpp](https://github.com/ggerganov/llama.cpp)项目中的[release版本](https://github.com/ggerganov/llama.cpp/releases/tag/b4604),找到llama-b4604-bin-win-avx-x64.zip并解压,将以下文件复制到项目的server文件夹下

![界面截图](image/server目录.png)

3. 到[魔搭社区](https://modelscope.cn/models)下载模型，将模型文件放到项目的models文件夹下,注意模型必须为gguf格式，这样才能被llama.cpp识别
4. 运行AIChatBox.exe


## 📦 环境要求

- Windows 10/11 64位
- Visual Studio 2022 (需安装MFC组件)
- [llama.cpp](https://github.com/ggerganov/llama.cpp) 服务端
- 至少8GB可用内存

## 🛠 编译运行

1. 安装Visual Studio 2022，确保安装了MFC组件
2. 下载[llama.cpp](https://github.com/ggerganov/llama.cpp)项目中的[release版本](https://github.com/ggerganov/llama.cpp/releases/tag/b4604),找到llama-b4604-bin-win-avx-x64.zip并解压,将以下文件复制到项目的server文件夹下

![界面截图](image/server目录.png)

3. 到[魔搭社区](https://modelscope.cn/models)下载模型，将模型文件放到项目的models文件夹下,注意模型必须为gguf格式，这样才能被llama.cpp识别
4. 使用Visual Studio 2022打开项目，配置项目属性，将项目的平台工具集改为Visual Studio 2022 (v143)
5. 编译项目，运行

## 🔗 参考项目

- [llama.cpp](https://github.com/ggerganov/llama.cpp) - 用于本地推理的高效C++库
- [llamacpp-terminal-chat](https://github.com/hwpoison/llamacpp-terminal-chat) - 基于llama.cpp的终端聊天客户端
