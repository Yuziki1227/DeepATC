# 本项目暂未开放使用

# DEEP ATC ✈️ - 基于 DeepSeek-R1:8B 的AI空中交通管制系统

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen)](https://www.python.org/)
[![Compatibility](https://img.shields.io/badge/Compatible%20with-Paper3D%20V6/MSFS%202024/XPLANE12-orange)]()

**Deep ATC** 是由 **DeepSeek-R1:8B** 大语言模型驱动的下一代智能空中交通管制解决方案，专为飞行模拟爱好者设计，兼容主流飞行模拟平台。


## ✨ 核心功能
- 🚀 **AI 实时管制指令生成**
  基于 DeepSeek-R1:8B 的自然语言处理能力，动态生成符合ICAO标准的管制指令(暂不支持FAA地区)
- 🌐 **多平台兼容支持**
  无缝集成 Paper3D V6 / Microsoft Flight Simulator 2024 / X-Plane 12
- 🎮 **自然语言交互**
  支持语音输入与文本指令的混合交互模式
- ⚡ **低延迟架构**
  通过模型量化技术实现8B参数的实时推理（RTX 4060+ 可达 <200ms 响应）
- 🔧 **可扩展接口**
  提供 REST API 和 SimConnect/X-Plane 插件支持

## 📥 快速安装
- 克隆仓库：
  - `git clone https://github.com/Yuziki1227/ai-atc.git`
  - `cd ai-atc`
- 安装依赖：
  - `pip install -r requirements.txt`
- 配置 DeepSeek API 密钥：
  - `echo "DEEPSEEK_API_KEY=your_api_key_here" > .env`
- 启动程序：
  - `python main.py --simulator=msfs2024`  # 可选参数: paper3d_v6 / xplane12

## 🛠️ 使用说明
### 配置模拟器
- 确保已安装对应平台的SDK/插件系统

### 启动 Deep ATC
- 根据不同平台选择运行模式：
  - `python main.py --simulator=msfs2024 --voice_input`  # 启用语音识别

### 交互示例
- Pilot: "Beijing Approach, CCA101 requesting descent instructions"
- AI ATC: "CCA101, descend and maintain FL180, contact Tower on 118.7"

- Pilot: "首都塔台晚上好, 国航101正在ILS进近跑道36右, 请求降落引导"
- AI ATC: "国航101, 首都塔台收到你的请求, 地面静风, 跑道36L可以落地"
-
## 📚 模拟器兼容性矩阵
| 模拟平台      | 测试版本    | 支持功能                           |
|---------------|-------------|------------------------------------|
| Paper3D V6    | 6.2.1+      | 完整 ATC 指令链/冲突检测           |
| MSFS 2024     | 1.35.12+    | 语音交互/动态天气适配               |
| X-Plane 12    | 12.1.0+     | 多跑道支持/自定义航路生成           |

## 🤝 参与贡献
欢迎通过以下方式参与项目：
- 提交 Pull Request 改进核心功能
- 在 Issues 报告问题
- 参与 Discussions 的功能设计

## 📜 许可证
本项目基于 MIT License 开源，模型使用需遵守 DeepSeek 模型协议。

## 🙏 致谢
- 感谢 DeepSeek-R1:8B 提供强大的核心支持，其开源精神为本项目带来了无限可能！
- 受 Paper3D/MSFS/X-Plane 生态启发

让每一次虚拟飞行都获得专业级的管制体验！ ✈️🗣️
