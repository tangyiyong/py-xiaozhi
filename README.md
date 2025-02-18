# py-xiaozhi

## 项目简介
py-xiaozhi 是一个使用 Python 实现的小智语音客户端，旨在通过代码学习和在没有硬件条件下体验 AI 小智的语音功能。
本仓库是基于zhh827的[py-xiaozhi](https://github.com/zhh827/py-xiaozhi/tree/main)优化再新增功能

## 项目背景
- 原始硬件项目：[xiaozhi-esp32](https://github.com/78/xiaozhi-esp32)
- 参考 Python 实现：[py-xiaozhi](https://github.com/zhh827/py-xiaozhi/tree/main)

## 演示
- [Bilibili 演示视频](https://b23.tv/GbXeLHX)

## 功能特点
- 语音交互
- 图形化界面
- 音量控制
- 会话管理
- 加密音频传输

## 环境要求
- Python 3.8+（推荐 3.12）
- Windows/Linux/macOS

## 安装依赖

### Windows 环境
1. 克隆项目
```bash
git clone https://github.com/Huang-junsen/py-xiaozhi.git
cd py-xiaozhi
```

2. 安装 Python 依赖
```bash
pip install -r requirements.txt
```

3. 拷贝 opus.dll
- 将 `opus.dll` 拷贝到 `C:\Windows\System32` 目录

### Linux/macOS 环境
```bash
git clone https://github.com/Huang-junsen/py-xiaozhi.git
cd py-xiaozhi
pip3 install -r requirements.txt
```

## 运行
```bash
python main.py
```

## 使用说明
- 启动应用程序后，GUI 界面会自动连接
- 点击并按住 "按住说话" 按钮开始语音交互
- 松开按钮结束语音输入

## 已知问题
- 需要稳定的网络连接
- 音频设备兼容性可能存在差异

## 已实现功能

- [x] 优化了 goodbye 后无法重连问题
- [x] 新增 GUI 页面，无需在控制台一直按空格
- [x] 拆分代码，封装为类，各司其职
- [x] 控制windows音量大小（mac/linux需要自行实现）
- [x] MAC_ADDR 自动获取（解决mac地址冲突问题）

## 待实现功能

- [ ] WebSocket 通信（开发中）
- [ ] 新 GUI （Electron）
- [ ] 第三方音乐库

## 贡献
欢迎提交 Issues 和 Pull Requests！

## 免责声明
本项目仅用于学习和研究目的，不得用于商业用途。

## 感谢以下开源人员
[Xiaoxia](https://github.com/78)
[zhh827](https://github.com/zhh827)