# D35 | 2026-06-30 | Project Setup

> **Project:** Smart Environmental Monitoring System  
> **Countdown:** D35 / 35  
> **Date:** 2026-06-30  
> **Phase:** Project Initialization & Development Environment Setup

---

# 阶段（Phase）

## Phase 1：项目启动与开发环境搭建（2026-06-30 ~ 2026-07-02）

### 阶段目标

- 确认项目最终方案
- 搭建 ESP32 开发环境
- 建立 GitHub 工程仓库
- 建立项目开发规范
- 验证 ESP32 能够正常烧录程序

---

# 当日任务（Today's Tasks）

| Task | Status |
|------|:------:|
| 确认项目整体方案 | ✅ |
| 建立 GitHub Repository | ✅ |
| 规划项目目录结构 | ✅ |
| 安装 Arduino IDE | ✅ |
| 安装 ESP32 开发板支持包 | ✅ |
| 安装 CP2102 USB Driver | ✅ |
| 成功识别 ESP32（COM5） | ✅ |
| 编译 Blink 示例程序 | ✅ |
| 烧录 Blink 程序 | ✅ |
| 板载 LED 闪烁测试 | ✅ |
| 建立每日开发日志规范 | ✅ |

---

# 完成情况（Progress）

## 一、文字说明（Description）

今天完成了整个项目的启动工作。

首先完成了 Arduino IDE 的安装，并成功安装 ESP32 开发板支持包。

随后由于 Windows 未安装 CP2102 USB 转串口驱动，ESP32 无法正常烧录程序。经过排查并安装 Silicon Labs 官方 CP210x VCP Driver 后，开发板成功被系统识别为 **COM5**。

之后完成了 ESP32 Blink 示例程序的编译与烧录，开发板板载 LED 能够按照 **1 秒亮、1 秒灭** 的方式持续闪烁，证明 ESP32 开发环境搭建成功。

同时完成 GitHub Repository 建立、Git 本地仓库初始化、Commit、Pull、Push 等工程开发流程，建立了整个项目统一的开发日志（Log）管理规范。

---

## 二、图片（Photos）

> 将今天拍摄的照片直接拖入 Markdown。

建议上传：

- ESP32 开发板照片
- Arduino IDE 烧录成功截图
- LED 闪烁照片
- GitHub Repository 截图

---

## 三、视频（Videos）

> 将今天录制的视频直接拖入 Markdown。

建议上传：

- Blink LED 演示视频
- ESP32 烧录演示视频

---

## 四、代码（Code）

### ESP32 Blink Test

```cpp
// ESP32 Blink Test

const int ledPin = 2;   // ESP32板载LED通常连接GPIO2

void setup() {
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);   // LED亮
  delay(1000);

  digitalWrite(ledPin, LOW);    // LED灭
  delay(1000);
}
```

---

# 备注（Notes）

## 遇到的问题

### 问题一：ESP32 无法烧录程序

**现象：**

```
Failed to connect to ESP32
No serial data received
```

**原因：**

Windows 未安装 CP2102 USB 转串口驱动。

**解决方案：**

安装 Silicon Labs 官方 CP210x VCP Driver，设备成功识别为 COM5，问题解决。

---

### 问题二：Git Push 无法连接 GitHub

**现象：**

```
Failed to connect to github.com via 127.0.0.1
```

**原因：**

Git 使用了失效的代理配置。

**解决方案：**

清除代理配置，重新同步远程仓库，成功完成 Push。

---

# 今日成果（Today's Achievement）

✅ ESP32 开发环境搭建完成

✅ Arduino IDE 配置完成

✅ CP2102 驱动安装完成

✅ ESP32 成功识别（COM5）

✅ Blink 程序烧录成功

✅ 板载 LED 闪烁正常

✅ GitHub 工程仓库建立完成

✅ Git 工作流程验证完成

✅ 项目开发日志规范建立完成

---

# 下一工作日（D34）

## 计划任务

- 检查开发环境完整性
- 确认采购订单状态
- 完善项目目录结构
- 为 AHT20 温湿度传感器开发做好准备

---

**Project Status：**

🟩 Phase 1 Started

**Overall Progress：**

`1 / 35 Working Days Completed`