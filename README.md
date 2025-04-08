# 智能家居语音助手

基于多模态交互的智能家居控制系统，支持语音/文本指令识别、场景感知和设备推荐。

## 功能特性

- 🎙️ 语音识别控制（Vosk引擎）
- 📱 多AI引擎支持（百度千帆/讯飞星火/豆包/Deepseek）
- 🏠 场景感知（安防/清洁/厨房等7大场景）
- 🧠 个性化推荐（基于用户画像+时间+地域）
- 📊 设备使用统计与分析

## 文件结构
smart_home/
├── core/ # 核心模块
│ ├── init.py
│ ├── cli_main.py # 主程序入口
│ ├── prompt_engine.py # 提示词管理
│ └── voice_agent.py # 语音处理
├── models/ # 语音模型
│ └── vosk-model-small/ # Vosk小型语音模型
├── data/
│ └── user_profiles/ # 用户数据存储
├── requirements.txt # 依赖库
└── README.md

复制

## 快速开始

1. 安装依赖：
   ```bash
   pip install -r requirements.txt
下载语音模型：

bash
复制
wget https://alphacephei.com/vosk/models/vosk-model-small-zh-cn-0.22.zip
unzip vosk-model-small-zh-cn-0.22.zip -d models/
配置API密钥：

bash
复制
export QIANFAN_API_KEY="your_api_key"
export SPARK_API_KEY="your_api_key" 
运行程序：

bash
复制
python core/cli_main.py
交互方式
复制
请选择输入方式:
1. 文本输入
2. 语音输入
3. 退出

>> 说"打开空调"或输入"灯光 电视"
开发配置
Python 3.8+

需要麦克风设备（语音模式）

各AI平台API申请：

百度千帆

讯飞星火
