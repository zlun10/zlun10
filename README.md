### Hi there, I'm zlun 👋

嵌入式固件工程师，做语音对讲类产品的拓展 IC 固件。

- 📍 中国 · GitHub 2024-04 加入
- 🛠 主力语言 C，平台 ARM Cortex-M0+（CW32L01x 系列），Keil MDK + Arm Compiler 6（armclang）
- 🔌 通过 AT 指令驱动外部语音模组，并在拓展 IC 上自己实现按键、显示、NV 存储等功能
- 🐞 调试链：SEGGER J-Link / SWD 烧录，运行日志走 RTT，串口时序用逻辑分析仪抓
- 🤖 同时用多个 AI 编码工具在同一份仓库上干活，关心"知识存在哪、换工具会不会丢"

## 🧰 技术栈

<div align="left">
  <img src="https://skillicons.dev/icons?i=c,cpp,py,powershell,git,vscode" alt="skills" />
</div>

## 🏗 日常在解决的事

**分层与多产品**
`chip → drv → hal → bsp → app` 单向分层，同一套驱动靠 BSP 配置与产品宏跑多款板子；每个产品一个独立工程，命令行脚本一次产出 debug / release。

**少上实机**
逻辑尽量先在 PC 侧验证：主机端单元测试 + 显示布局仿真，实机只用来确认时序与电气行为，减少"改一版烧一次"的来回。

**把流程做成脚本**
构建、烧录、抓日志、版本同步串成闭环，改动可以批量验证而不是手工点 IDE。

**跨工具的规范只写一份**
协作与编码规则集中在唯一规范源，各 AI 工具的入口文件只做指向它薄入口，由校验脚本检查漂移 —— 工具可以换，规范不该有第二份副本。

## 🌱 也在玩

Vue 3 + Service Worker 的 PWA 小工具，和个人主页本身。
