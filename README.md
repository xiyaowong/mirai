<div align="center">
   <img width="160" src="docs/mirai.png" alt="logo"></br>

   <img width="95" src="docs/mirai.svg" alt="title">

----

![Gradle CI](https://github.com/mamoe/mirai/workflows/Gradle%20CI/badge.svg?branch=master)
[![Download](https://api.bintray.com/packages/him188moe/mirai/mirai-core/images/download.svg)](https://bintray.com/him188moe/mirai/mirai-core/)
[![Gitter](https://badges.gitter.im/mamoe/mirai.svg)](https://gitter.im/mamoe/mirai?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

mirai 是一个在全平台下运行，提供 QQ Android 协议支持的高效率机器人库

这个项目的名字来源于
     <p><a href = "http://www.kyotoanimation.co.jp/">京都动画</a>作品<a href = "https://zh.moegirl.org/zh-hans/%E5%A2%83%E7%95%8C%E7%9A%84%E5%BD%BC%E6%96%B9">《境界的彼方》</a>的<a href = "https://zh.moegirl.org/zh-hans/%E6%A0%97%E5%B1%B1%E6%9C%AA%E6%9D%A5">栗山未来(Kuriyama <b>mirai</b>)</a></p>
     <p><a href = "https://www.crypton.co.jp/">CRYPTON</a>以<a href = "https://www.crypton.co.jp/miku_eng">初音未来</a>为代表的创作与活动<a href = "https://magicalmirai.com/2019/index_en.html">(Magical <b>mirai</b>)</a></p>
图标以及形象由画师<a href = "https://github.com/DazeCake">DazeCake</a>绘制
</div>


## mirai

**[English](README-eng.md)**  

## 声明

### 一切开发旨在学习，请勿用于非法用途

- mirai 是完全免费且开放源代码的软件，仅供学习和娱乐用途使用
- mirai 不会通过任何方式强制收取费用，或对使用者提出物质条件
- mirai 由整个开源社区维护，并不是属于某个个体的作品，所有贡献者都享有其作品的著作权。
```
除本页的 Gitter 讨论组外，Mirai 在各个平台均没有任何所谓官方交流群或论坛, 请不要轻信任何所谓学习, 交流群, 不造谣不传谣不信谣从我做起
```

### 许可证

    Copyright (C) 2019-2020 Mamoe Technologies and contributors.

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU Affero General Public License as
    published by the Free Software Foundation, either version 3 of the
    License, or (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU Affero General Public License for more details.

    You should have received a copy of the GNU Affero General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>.

`mirai` 采用 `AGPLv3` 协议开源。为了整个社区的良性发展，我们**强烈建议**您做到以下几点：

- **间接接触（包括但不限于使用 `Http API` 或 跨进程技术）到 `mirai` 的软件使用 `AGPLv3` 开源**
- **不鼓励，不支持一切商业使用**

鉴于项目的特殊性，开发团队可能在任何时间**停止更新**或**删除项目**。

### **mirai 的形象图及项目图标都拥有著作权保护。**
**在未经过允许的情况下，任何人都不可以使用形象图和图标，或本文初的有关 mirai 名称来历的介绍原文，用于商业用途或是放置在项目首页，或其他未许可的行为。**

### 衍生软件需声明引用

- 若引用 mirai 发布的软件包而不修改 mirai，则衍生项目需在描述的任意部位提及使用 mirai。
- 若修改 mirai 源代码再发布，或参考 mirai 内部实现发布另一个项目，则衍生项目必须在**文章首部**或 'mirai' 相关内容**首次出现**的位置**明确声明**来源于本仓库 (`https://github.com/mamoe/mirai`)。不得扭曲或隐藏免费且开源的事实。

## 协议支持

<details>
  <summary>支持的协议列表</summary>

| 消息相关                    | 支持              |
|:----------------------|:----------------|
| 文字                  | 群聊 \| 好友 \| 临时会话 |
| 原生表情                  | 群聊 \| 好友 \| 临时会话 |
| 图片 上传 / 发送 / 解析 (最大 20M)           | 群聊 \| 好友 \| 临时会话 |
| 图片下载           | 群聊 \| 好友 \| 临时会话 |
| XML，JSON 等富文本消息           | 群聊 \| 好友 \| 临时会话 |
| 长消息 (5000 字符 + 50 图片) | 群聊               |
| 引用回复                  | 群聊 \| 好友 \| 临时会话 |
| 合并转发 (最大 200 条)                  | 群聊  |
| 撤回                  | 群聊 \| 好友 \| 临时会话 |
| At (含 At 全体成员)                  | 群聊 |
| 撤回群员消息                  | 群聊 |

| 群相关                    |
|:----------------------|
| 完整群列表; 完整群成员列表|
| 群员权限获取|
| 禁言群员; 全员禁言; 禁言时间获取|
| 群公告管理(获取，发布，删除)|
| 群设置(自动审批，入群公告，坦白说，成员邀请，匿名聊天)|
| 处理入群申请; 移除群员 |

| 好友相关 |
|:----|
| 完整好友列表 |
| 处理新好友申请 |

</details>

#### 不会支持的协议
- 金钱相关，如点赞、收付款
- 敏感操作，如主动添加好友、主动加入群、主动邀请好友加群
- 安全相关，获取账号登录凭证(token，cookie等)

**一切开发旨在学习，请勿用于非法用途**

## 开始

### 文档

**对于一般使用者, 更建议使用 [Mirai Console](https://github.com/mamoe/mirai-console)。拥有更完善的文档。**

- 快速上手：[quickstart](docs/guide_quick_start.md)
- 开发文档：[docs/mirai.md](docs/mirai.md)
- 常见问题: [docs/FAQ.md](docs/FAQ.md)
- 更新日志: [CHANGELOG](https://github.com/mamoe/mirai/blob/master/CHANGELOG.md) 或 [release](https://github.com/mamoe/mirai/releases)
- 开发计划: [milestones](https://github.com/mamoe/mirai/milestones)
- 贡献: [CONTRIBUTING](CONTRIBUTING.md)

### 使用者

- [mirai-console](https://github.com/mamoe/mirai-console) 支持插件的控制台服务端，支持PC和Android平台 **本模块正在开发中**
- [awesome-mirai](https://github.com/project-mirai/awsome-mirai/blob/master/README.md) **mirai相关项目合集**

#### 从其他平台迁移

- 酷Q的插件可以在 `mirai` 中加载，详见 [Mirai Native](https://github.com/iTXTech/mirai-native)
- 使用 `酷Q HTTP API` 的插件将可以在 `mirai` 中通过`CQHTTP Mirai`加载，详见 [cqhttp-mirai](https://github.com/yyuueexxiinngg/cqhttp-mirai)

### 开发者

开发交流：[![Gitter](https://badges.gitter.im/mamoe/mirai.svg)](https://gitter.im/mamoe/mirai?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

#### 使用 mirai-console 服务端，为 mirai-console 开发插件

官方支持 SDK 列表:

- `Java`，`Kotlin` 等 JVM 语言： 为 [mirai-console](https://github.com/mamoe/mirai-console) 直接编写插件并与其他插件开发者合作共享
- `Kotlin Script`： [mirai-kts](https://github.com/iTXTech/mirai-kts) 支持使用 `kts` 编写插件，享受 `Kotlin` 带来的一切便利（**仅 OpenJDK 8 以上环境，不支持 Android**）
- `C`，`C++` 等原生语言： [mirai-native](https://github.com/iTXTech/mirai-native) 支持酷 Q 插件在 mirai 上运行 **(仅限 `Windows 32 位 JRE`/支持 `Wine`)**
- `JavaScript`： [mirai-js](https://github.com/iTXTech/mirai-js) 支持使用 `JavaScript` 编写插件并**直接**与 mirai 交互
- *Http*：使用由 [mirai-api-http](https://github.com/mamoe/mirai-api-http) 提供的 http 接口进行接入

<details>
  <summary>社区支持的 SDK 列表</summary>

基于 `mirai-core` (独立使用):
- `Lua`: [lua-mirai](https://github.com/only52607/lua-mirai) 基于 mirai-core 的 Lua SDK，并提供了 Java 扩展支持，可在 Lua 中调用 Java 代码开发机器人


基于 `mirai-http-api` (配合 [mirai-console](https://github.com/mamoe/mirai-console)):

- `Python`: [Graia Framework](https://github.com/GraiaProject/Application) 基于 `mirai-api-http` 的机器人开发框架
- `JavaScript`(`Node.js`): [node-mirai](https://github.com/RedBeanN/node-mirai) mirai 的 Node.js SDK
- `Go`: [gomirai](https://github.com/Logiase/gomirai) 基于 mirai-api-http 的 GoLang SDK
- `Mozilla Rhino`: [mirai-rhinojs-sdk](https://github.com/StageGuard/mirai-rhinojs-sdk) 为基于 Rhino(如 Auto.js 等安卓 app 或运行环境)的 JavaScript 提供简单易用的 SDK
- `C++`: [mirai-cpp](https://github.com/cyanray/mirai-cpp) mirai-http-api 的 C++ 封装，方便使用 C++ 开发 mirai-http-api 插件
- `C++`: [miraipp](https://github.com/Chlorie/miraipp-template) mirai-http-api 的另一个 C++ 封装，使用现代 C++ 特性，并提供了较完善的说明文档
- `C#`: [mirai-CSharp](https://github.com/Executor-Cheng/mirai-CSharp) 基于 mirai-api-http 的 C# SDK
- `Rust`: [mirai-rs](https://github.com/HoshinoTented/mirai-rs) mirai-http-api 的 Rust 封装
- `TypeScript`: [mirai-ts](https://github.com/YunYouJun/mirai-ts) mirai-api-http 的 TypeScript SDK，附带声明文件，拥有良好的注释和类型提示，也可作为 JavaScript SDK 使用。
- `易语言`: [e-mirai](https://github.com/only52607/e-mirai) mirai-api-http 的 易语言 SDK，使用全中文环境开发插件，适合编程新手使用。
- `.Net/C#`: [Hyperai](https://github.com/theGravityLab/ProjHyperai) 从 mirai-api-http 对接到机器人开发框架再到开箱即用的插件式机器人程序一应俱全。

</details>

#### 使用 mirai-core 为第三方依赖库引入项目

Demos: [mirai-demos](https://github.com/mamoe/mirai-demos)

- `Kotlin` 简略版： [mirai Guide - Quick Start](/docs/guide_quick_start.md)
- `Kotlin` 新手版： [mirai Guide - Getting Started](/docs/guide_getting_started.md)
- `Java`： 查看上述 Demos

## [贡献](CONTRIBUTING.md)

我们欢迎一切形式的贡献。  
我们也期待有更多人能加入 mirai 的开发。  

若在使用过程中有任何疑问，可提交 `issue` 或是[邮件联系](mailto:support@mamoe.net). 我们希望 mirai 变得更易用.

您的 `star` 是对我们最大的鼓励(点击项目右上角)

### 加入 mirai 开发组
若您有意加入 mirai, mirai-console 和相关社区开发, 请 [邮件联系](mailto:support@mamoe.net) (`support@mamoe.net`), 并附加相关开发经验证明.

## 鸣谢

> [IntelliJ IDEA](https://zh.wikipedia.org/zh-hans/IntelliJ_IDEA) 是一个在各个方面都最大程度地提高开发人员的生产力的 IDE，适用于 JVM 平台语言。

特别感谢 [JetBrains](https://www.jetbrains.com/?from=mirai) 为开源项目提供免费的 [IntelliJ IDEA](https://www.jetbrains.com/idea/?from=mirai) 等 IDE 的授权  
[<img src=".github/jetbrains-variant-3.png" width="200"/>](https://www.jetbrains.com/?from=mirai)
