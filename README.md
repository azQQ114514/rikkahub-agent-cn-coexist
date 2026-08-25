<div align="center">

# RikkaHub Agent 中文共存版

**你的设备，已汉化。**

基于 [RikkaHub Agent](https://github.com/ExTV/rikkahub-agent) 二次开发的中文增强版：全量简体中文本地化、工作区文件导入上限放开至 10GB、独立包名可与官方原版并存安装。所有上游功能与工具能力完整保留。

</div>

---

## 这是什么

上游链路：[RikkaHub](https://github.com/rikkahub/rikkahub)（原版客户端）→ [ExTV/rikkahub-agent](https://github.com/ExTV/rikkahub-agent)（Agent 增强版，80+ 设备工具、工作流、计划任务、内置浏览器、Linux 工作区等）→ 本项目（在其之上的中文版）。

本仓库基于 RikkaHub Agent **v2.4.10** 制作，不改动任何核心功能逻辑，只做本地化与限制放宽。

## 相对上游改了什么

### 1. 全量中文化
- 界面资源 2100+ 条目全部翻译为简体中文
- Compose 硬编码界面文本插桩汉化（覆盖资源文件够不到的界面）
- 系统权限说明人性化重写，用大白话讲清楚每个权限干什么
- 全量术语一致性审计（2700+ 条目交叉核对，统一术语口径）
- 翻译资料随仓库公开（翻译库与修改清单见 docs/ 目录）

### 2. 导入上限：256MB → 10GB
- 官方限制工作区单次文件导入最大 256MB，本版放开至 10GB
- 便于导入大型语料、资料文件到工作区

### 3. 与官方版共存安装
- 独立包名（excp.rikkahub.zhcn），可与官方 RikkaHub / RikkaHub Agent 同时安装、互不影响
- 使用独立签名（仅 v2/v3 方案），与官方签名不同；若已装官方版无需卸载，直接并存

## 安装

前往 [Releases](../../releases) 下载 APK，直接安装即可。

## 致谢与免责声明

- 本项目与 RikkaHub 官方维护者及 RikkaHub Agent（ExTV）维护者无关，问题请提给本仓库而不是上游
- 底层客户端、供应商抽象、UI 设计等一切功能归功于上游团队
- 上游版本更新较快，本分支内容可能落后于上游，请及时关注上游动态

## License

[AGPL-3.0](LICENSE)，继承自上游；本分支的全部修改以相同协议公开。
