<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4F46E5,100:06B6D4&height=130&section=header&animation=fadeIn" width="100%" alt="header" />

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=24&duration=3000&pause=800&color=4F46E5&center=true&vCenter=true&width=680&lines=ROS+2+Robotics+Engineer;Nav2+%7C+OpenCV+%7C+MQTT;%E8%AE%A9%E6%9C%BA%E5%99%A8%E4%BA%BA%E8%87%AA%E5%B7%B1%E8%B5%B0%E8%BF%87%E5%8E%BB" alt="Typing SVG" />

# 你好，我是曾煜翔 👋

**ROS 2 机器人开发 · 导航集成 · 机器视觉**

[![Blog](https://img.shields.io/badge/Blog-zeng417.github.io-4F46E5?style=for-the-badge&logo=jekyll&logoColor=white)](https://zeng417.github.io)
[![Email](https://img.shields.io/badge/Email-1277254986%40qq.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:1277254986@qq.com)

<img src="https://komarev.com/ghpvc/?username=zeng417&label=PROFILE+VIEWS&style=for-the-badge&color=4F46E5" alt="Profile views" />

</div>

---

## 🧭 关于我

把机器人从「能跑通」推到「能上线」的本科生，喜欢把过程写清楚。

- 🔭 **在做什么**：天轶 2.5 室内消防设施巡检机器人 —— 定点巡检导航、底盘话题对接、激光建图与重定位
- 🏆 **拿过什么**：第二届世界人形机器人运动会「园林场景赛」冠军（2026.08）
- 🧠 **关注方向**：Nav2 导航集成、多传感器融合、OpenCV 视觉、IoT 通信
- 📝 **写文章**：ROS 2 / MQTT / 强化学习笔记 → [我的博客](https://zeng417.github.io)
- 🌱 **正在补**：行为树与参数调优、真实机器人上的异常恢复

---

## 🏅 荣誉

| 时间 | 奖项 |
| :--- | :--- |
| 2026.08 | 第二届世界人形机器人运动会 · 园林场景赛 **冠军** |
| 2026 | 第十七届蓝桥杯 C/C++ 程序设计 · 省级 **二等奖** |

---

## 🛠 技术栈

<div align="center">

![ROS 2](https://img.shields.io/badge/ROS_2-Jazzy-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

</div>

---

## 🚀 代表项目

### 🎯 qr-barcode-scanner · 实时二维码 / 一维码识别

摄像头实时识码工具，解决「深色背景、贴边、模糊、远距离」这些真实场景下的漏检。

| 模块 | 实现 |
| :--- | :--- |
| 多引擎解码 | zxing-cpp 主引擎 + pyzbar + OpenCV，按内容与位置去重 |
| 鲁棒性 | 定位内环透视校正 + 补白重试，单帧最多 4 个候选区域 |
| 数据 | 扫码事件持久化 SQLite，自动导出 CSV，失败缓存重试 |
| 集成 | 识别结果可经 MQTT 推送到 Broker，接入 IoT / 机器人 |

→ [github.com/zeng417/qr-barcode-scanner](https://github.com/zeng417/qr-barcode-scanner)

### 🤖 天轶 2.5 · 室内消防设施巡检导航

基于 ROS 2 Jazzy 的定点巡检导航应用：沿预设路线抵达消防设施检测位，到点校验、受阻自恢复、返程分段续行。

- 巡检任务编排：按设施分布配置路径与目标点位，串起固定路线的多点位导航流程
- 接口衔接：Python 对接底盘 ROS 话题，完成应用层与执行层的消息交互
- 定位与避障：激光雷达建图 + 重定位恢复位姿，结合平台自动避障能力落地

→ 设计细节见博客：[基于 ROS 2 的天轶 2.5 消防巡检机器人导航模块设计与实践](https://zeng417.github.io/posts/tianyi25-fire-inspection-nav/)

### 📰 weekly-website · 具身智能周刊

每周精选行业洞察、开源项目与论文速递，VitePress 构建，已更新至第 39 期。

→ [weekly-website-nine.vercel.app](https://weekly-website-nine.vercel.app)

---

## 📝 最近在写

<!-- BLOG-POST-LIST:START -->
- [点对点、轨道与自主导航：三种「自己走过去」到底差在哪](https://zeng417.github.io/posts/robot-navigation-modes/)
- [基于 ROS 2 的天轶 2.5 消防巡检机器人导航模块设计与实践](https://zeng417.github.io/posts/tianyi25-fire-inspection-nav/)
- [MQTT 协议入门：用「订阅报纸」的方式理解物联网通信](https://zeng417.github.io/posts/mqtt-protocol-intro/)
<!-- BLOG-POST-LIST:END -->

---

## 📊 GitHub 数据

<div align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=zeng417&show_icons=true&theme=tokyonight&hide_border=true&locale=cn&count_private=true" alt="GitHub Stats" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zeng417&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" />

<img width="100%" src="https://streak-stats.demolab.com?user=zeng417&theme=tokyonight&hide_border=true&locale=zh-Hans" alt="Streak Stats" />

</div>

---

## 📫 联系我

- 🌐 博客 · <https://zeng417.github.io>
- ✉️ 邮箱 · <1277254986@qq.com>
- 💬 GitHub · [@zeng417](https://github.com/zeng417)

<div align="center">
  <sub>「记录踩过的坑，也记录想明白的瞬间。」</sub>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,100:4F46E5&height=110&section=footer" width="100%" alt="footer" />
