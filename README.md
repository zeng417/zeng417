<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7C3AED,100:EC4899&height=200&section=header&text=zeng417&fontSize=64&fontColor=ffffff&fontAlignY=36&desc=ROS%202%20%C2%B7%20Nav2%20%C2%B7%20Computer%20Vision&descAlignY=58&descSize=18" width="100%" alt="header" />

<a href="https://github.com/zeng417">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=7C3AED&center=true&vCenter=true&width=620&lines=ROS+2+Robotics+Engineer;Nav2+%7C+OpenCV+%7C+MQTT;%E8%AE%A9%E6%9C%BA%E5%99%A8%E4%BA%BA%E8%87%AA%E5%B7%B1%E8%B5%B0%E8%BF%87%E5%8E%BB" alt="Typing SVG" />
</a>

</div>

## 关于我

<table>
  <tr>
    <td width="50%" valign="top">
      <b>我在做什么</b><br/>
      天轶 2.5 室内消防设施巡检机器人：定点巡检导航、底盘话题对接、激光建图与重定位。
    </td>
    <td width="50%" valign="top">
      <b>技术关注</b><br/>
      Nav2 导航集成 · OpenCV 视觉 · ROS 2 通信 · MQTT 物联网
    </td>
  </tr>
  <tr>
    <td colspan="2" valign="top">
      <b>联系我</b><br/>
      <a href="mailto:1277254986@qq.com">Email</a> · <a href="https://zeng417.github.io">博客</a>
    </td>
  </tr>
</table>

## 技术栈

**语言与基础**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**框架与工具**

![ROS 2](https://img.shields.io/badge/ROS_2-Jazzy-22314E?style=for-the-badge&logo=ros&logoColor=white)
![Nav2](https://img.shields.io/badge/Nav2-1F6FEB?style=for-the-badge)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)

## 代表项目

### 📄 paper-cards · 具身智能论文知识卡片库

按 CEAI 2025「具身智能十五大重点方向」整理论文，每篇拆成速览卡、精读笔记、全文翻译与代码四份材料。

| 模块 | 实现 |
| :--- | :--- |
| 卡片结构 | 一篇论文 = README 速览卡 + reading-notes 精读 + translation 全文翻译 + 代码入口 |
| 体系划分 | 00 大模型基础 + 01–15 具身智能十五大方向，每方向预留 3 篇经典论文索引位 |
| 收录进度 | 已整理 10 篇论文，覆盖 8 个方向：多模态感知、自主学习、具身大模型、世界模型、操作、导航、强化学习自适应控制 |
| 协作流程 | templates/ 三份模板 + scripts/add-paper.py 一键生成骨架，CONTRIBUTING.md 约定提交规范 |

→ [github.com/yuanjingea/paper-cards](https://github.com/yuanjingea/paper-cards)

### 🤖 天轶 2.5 · 室内消防设施巡检导航

基于 ROS 2 Jazzy 的定点巡检导航应用：沿预设路线抵达消防设施检测位，到点校验、受阻自恢复、返程分段续行。

- **任务编排**：按设施分布配置路径与目标点位，串起固定路线的多点位导航流程
- **接口衔接**：Python 对接底盘 ROS 话题，完成应用层与执行层的消息交互
- **定位避障**：激光雷达建图 + 重定位恢复位姿，结合平台自动避障能力落地

→ 代码主仓库：[AJXING123/tianyi25-fire-inspection](https://github.com/AJXING123/tianyi25-fire-inspection)（第一贡献者）
→ 设计细节：[基于 ROS 2 的天轶 2.5 消防巡检机器人导航模块设计与实践](https://zeng417.github.io/posts/tianyi25-fire-inspection-nav/)

### 🎯 qr-barcode-scanner · 实时二维码 / 一维码识别

摄像头实时识码，专门解决「深色背景、贴边、模糊、远距离」下的漏检。

| 模块 | 实现 |
| :--- | :--- |
| 多引擎解码 | zxing-cpp 主引擎 + pyzbar + OpenCV，按内容与位置去重 |
| 鲁棒性 | 定位内环透视校正 + 补白重试，单帧最多 4 个候选区域 |
| 数据 | 扫码事件持久化 SQLite，自动导出 CSV，失败缓存重试 |
| 集成 | 识别结果可经 MQTT 推送 Broker，接入 IoT / 机器人 |

→ [github.com/zeng417/qr-barcode-scanner](https://github.com/zeng417/qr-barcode-scanner)

### 📰 weekly-website · 具身智能周刊

每周精选行业洞察、开源项目与论文速递，VitePress 构建，已更新至第 39 期。

→ [weekly-website-nine.vercel.app](https://weekly-website-nine.vercel.app)

## 最近在写

<!-- BLOG-POST-LIST:START -->
- [点对点、轨道与自主导航：三种「自己走过去」到底差在哪](https://zeng417.github.io/posts/robot-navigation-modes/)
- [基于 ROS 2 的天轶 2.5 消防巡检机器人导航模块设计与实践](https://zeng417.github.io/posts/tianyi25-fire-inspection-nav/)
- [MQTT 协议入门：用「订阅报纸」的方式理解物联网通信](https://zeng417.github.io/posts/mqtt-protocol-intro/)
<!-- BLOG-POST-LIST:END -->

## 🎯 接下来

- 把巡检导航从「能跑通」做到「可复现」：参数、日志、异常恢复
- 补行为树与 Nav2 参数调优
- 复盘比赛与项目，继续更博客

<div align="center">
  <sub>「记录踩过的坑，也记录想明白的瞬间。」</sub>
</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:EC4899,100:7C3AED&height=110&section=footer" width="100%" alt="footer" />
