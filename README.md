
# Legado 第三方版本汇总

> Legado（阅读）第三方 Fork 版本信息汇总，方便用户选择适合自己的版本。
>
> 原版仓库：[gedoor/legado](https://github.com/gedoor/legado)（作者已停更）

---

## 版本继承关系

```
gedoor/legado（原版，作者停更）
  │
  ├── Rimchars/legado（Archive版）── 改动较大，不能覆盖原版
  │     └── refgd/legado（R版）── AI助手 + EPUB + 主题 + 漫画视频增强
  │
  ├── Luoyacheng/legado（Sigma/lyc版）── 原版基础上新增功能
  │     └── youfengknight/Legado_Max（Max版）── 功能最多最全
  │           └── Suml-1/Legado_Max（Max复刻版）── 主仓库的镜像
  │
  ├── HapeLee/legado-with-MD3（MD3版）── UI完全重写，Compose迁移中
  │
  └── LegadoTeam/legado（LegadoTeam版）── 社区团队接手维护
        └── LegadoTeam/Legado-Tauri（Tauri桌面版）── 完全独立的桌面端产品
```

---

## 各版本详情

### 1. 原版 Legado

| 项目 | 信息 |
|------|------|
| 仓库 | [gedoor/legado](https://github.com/gedoor/legado) |
| Stars | 46,881 |
| Forks | 5,785 |
| 包名 | `io.legado.app` |
| 状态 | 已停更 |
| 说明 | 最初的开源 Android 阅读器，作者 gedoor（庭前花开）因法律问题停更 |

### 2. Archive版

| 项目 | 信息 |
|------|------|
| 仓库 | [Rimchars/legado](https://github.com/Rimchars/legado) |
| 继承 | 独立分支（非直接 fork 显示） |
| 能否覆盖原版 | 不能（包名或签名已变） |
| 说明 | 原版的延续分支，README 保留原版但实际代码改动较大，不能覆盖安装原版 |

### 3. Sigma版（lyc版）

| 项目 | 信息 |
|------|------|
| GitHub | [Luoyacheng/legado](https://github.com/Luoyacheng/legado) |
| Gitee | [lyc486/legado](https://gitee.com/lyc486/legado)（同项目） |
| Stars | 1,762 |
| Forks | 283 |
| 继承 | 原版 gedoor/legado |
| 说明 | 在原版基础上新增更多功能，为书源带来更多可能性 |

**版本类型：**

| 类型 | 包名 | 说明 |
|------|------|------|
| beta（测试版） | `io.legado.app`（同原版） | 可覆盖原版安装，更新频繁 |
| plus（正式版） | 共存包名 | 不覆盖原版，稳定阶段才更新 |

**社区：**

| 平台 | 链接 |
|------|------|
| Telegram | [@readsigma](https://t.me/readsigma) |
| Discord | [加入](https://discord.gg/VtUfRyzRXn) |
| 微信公众号 | legado_plus |

**下载：** [Gitee Releases](https://gitee.com/lyc486/legado/releases)

### 4. R版

| 项目 | 信息 |
|------|------|
| 仓库 | [refgd/legado](https://github.com/refgd/legado) |
| 继承 | Archive版（Rimchars/legado） |
| 说明 | 非 Sigma 线路，独立发展方向 |

**特色功能：**
- 重做主题管理（日间/夜间主题、背景图、界面颜色、主题导入导出和云端同步）
- 深化 EPUB 原生阅读（图片、注解、分页缓存、复杂样式、大文件导入）
- 增强 AI 助手（工具调用、书源搜索、书籍与章节读取、阅读记录查询、联网搜索）
- 优化发现页与订阅源页（统一源选择、订阅内容搜索、纯 URL 订阅源、合并入口）
- 改进漫画和视频体验（漫画阅读控件、视频直达播放页、详情/目录信息展示）

**版本类型：**

| 类型 | 包名 | 说明 |
|------|------|------|
| beta（测试版） | `io.legado.app`（同原版） | 可覆盖原版安装，更新频繁 |
| plus（正式版） | 共存包名 | 不覆盖原版，稳定阶段才更新 |

**社区：**

| 平台 | 链接 |
|------|------|
| Telegram | [@yuedur](https://t.me/yuedur) |

**下载：** [GitHub Releases](https://github.com/refgd/legado/releases)

### 5. Max版

| 项目 | 信息 |
|------|------|
| 主仓库 | [youfengknight/Legado_Max](https://github.com/youfengknight/Legado_Max) |
| 复刻仓库 | [Suml-1/Legado_Max](https://github.com/Suml-1/Legado_Max) |
| Stars | 主仓库 195 / 复刻 63 |
| 继承 | Sigma版（Luoyacheng/legado） |
| 说明 | 在 Sigma 基础上继续增强，功能最多最全 |

**版本类型：**

| 类型 | 包名 | 说明 |
|------|------|------|
| appLegacy版 | `io.legado.app`（同原版） | 可覆盖原版安装 |
| appMax版 | `io.legado.app.yuedu` | 共存包名 |
| appS版 | `io.legado.app.yuedu.a` | 共存包名 |

**特色功能：**
- **阅读体验增强** — 翻页速度自由调节、页眉页脚字体独立调节、波浪线/虚线下划线
- **调试与开发工具** — 集成调试工具台、代码编辑器增强、TTS源调试、字典/字重调试界面、调试日志悬浮球、书源检测新界面、代码编辑切换规则、查询规则快速跳转、帮助文档全局搜索、书签搜索
- **数据与记录管理** — 阅读记录四种视图、热力图日历、URL记录、完全备份支持、缓存管理界面增强、阅读记录搜索
- **UI/UX优化** — HTML封面模板引擎、主题批量操作、帮助文档选择器、帮助文档全局搜索、发现页useWeb展示、主题置顶功能、备份文件验证
- **功能扩展增强** — @webjs规则类型、智能导入、自动更新、JavaScript增强函数、向前向后预下载调节、JS Packages使用指南

**覆盖安装注意事项：**
- 从 MD3 版本备份的书架分组在 Max 版本中无法正常显示（MD3 自行修改了分组备份数据格式）
- 从 lyc/Sigma/Plus 版直接覆盖安装可能丢失书架和数据
- 建议安装前完整备份，如遇数据丢失：完全卸载后重装，再恢复备份

**社区：**

| 平台 | 链接 |
|------|------|
| Discord | [加入](https://discord.gg/VtUfRyzRXn) |

**下载：** [GitHub Releases（主仓库）](https://github.com/youfengknight/Legado_Max/releases)

> **注意：** Suml-1/Legado_Max 是主仓库的 fork，代码相同。建议认准 youfengknight 主仓库。

### 6. MD3版

| 项目 | 信息 |
|------|------|
| 仓库 | [HapeLee/legado-with-MD3](https://github.com/HapeLee/legado-with-MD3) |
| 继承 | 原版 + 参考 Sigma版 |
| 说明 | UI 完全重写，基于 Material Design 3，正在迁移至 Jetpack Compose |

**特色功能：**
- 全新 Material Design 3 设计界面，支持预测性返回手势与共享元素动画
- 更加个性化的阅读界面与菜单配置
- 详尽的阅读记录，支持时间轴与章节维度统计
- 更健全的漫画阅读、有声书与发现等界面体验
- 更多书架布局选择，针对平板端进行专门优化
- 新增书籍备注、智能伴生分组（自动归类已读/未读），支持手柄上下翻页

**注意事项：**
- 由于使用 Monet 引擎重构了主题系统，原版官方主题在此版本中不可用
- Android 12 以下设备暂不支持自定义主题与动态取色
- 书架分组备份数据格式与其他版本不兼容（Max 版已明确说明此问题）

**社区：**

| 平台 | 链接 |
|------|------|
| Telegram | [Legado with MD3](https://t.me/materado) |

**下载：** [GitHub Releases](https://github.com/HapeLee/legado-with-MD3/releases)

### 7. LegadoTeam版

| 项目 | 信息 |
|------|------|
| 仓库 | [LegadoTeam/legado](https://github.com/LegadoTeam/legado) |
| Stars | 243 |
| Forks | 83 |
| 组织 | [LegadoTeam](https://github.com/LegadoTeam)（GitHub 认证组织） |
| 官网 | [legadoteam.org](https://legadoteam.org) |
| 创建 | 2025年10月31日 |
| 说明 | 社区团队接手原版代码的延续维护版，以依赖升级和小幅修复为主 |

**版本类型：**

| 类型 | 包名 | 说明 |
|------|------|------|
| release | `io.legado.app`（同原版） | 可覆盖原版安装 |
| releaseA | `com.legado.app.releaseA` | 共存包名 |

**版本号示例：** 3.26.052802（2026年5月28日构建）

**特点：**
- 通过 GitHub Actions 自动构建发版
- 改动保守，与原版功能高度一致
- 持续进行依赖版本升级（json-path、viewpager2、material、activity 等）
- 适合从原版 3.25 平滑迁移

**下载：** [GitHub Releases](https://github.com/LegadoTeam/legado/releases)

### 8. LegadoTeam Tauri桌面版

| 项目 | 信息 |
|------|------|
| 主仓库 | [LegadoTeam/Legado-Tauri](https://github.com/LegadoTeam/Legado-Tauri) |
| 文档站 | [docs.legadoteam.org](https://docs.legadoteam.org) |
| Release仓库 | [LegadoTeam/Legado-Tauri-Release](https://github.com/LegadoTeam/Legado-Tauri-Release) |
| 文档仓库 | [LegadoTeam/Legado-docs](https://github.com/LegadoTeam/Legado-docs) |
| 组织 | [LegadoTeam](https://github.com/LegadoTeam) |
| 协议 | MIT |
| 说明 | 完全独立的桌面端产品，用 Tauri 框架（Rust + Web）构建 |

**特点：**
- 纯 JavaScript 书源（不兼容 Android 版书源）
- 全新 API 体系：`legado.dom.*` DOM解析、`legado.browser.*` 浏览器探测、`legado.image.*` 图片处理、`legado.http.*` HTTP请求
- 支持小说、漫画、视频、音乐/有声书
- 内置浏览器探测，能处理 JS 渲染页面和 Cloudflare 挑战
- 图片处理能力（解码、裁剪、拼接），适合漫画书源
- 命令行调试工具（CLI），便于开发和调试书源
- 支持鸿蒙平台
- 内置单元测试

**社区：**

| 平台 | 链接 |
|------|------|
| QQ一群 | 645815655（已满） |
| QQ二群 | 949235656（已满） |
| QQ三群 | 1107448928（可加入） |

**下载：** [GitHub Tauri Releases](https://github.com/LegadoTeam/Legado-Tauri-Release/releases)

---

## 包名速查表

| 版本 | 覆盖原版包名 | 共存包名 |
|------|-------------|---------|
| 原版 | `io.legado.app` | — |
| Sigma/lyc beta | `io.legado.app` | plus 版有 |
| R beta | `io.legado.app` | plus 版有 |
| Max appLegacy | `io.legado.app` | `io.legado.app.yuedu` / `io.legado.app.yuedu.a` |
| LegadoTeam release | `io.legado.app` | `com.legado.app.releaseA` |
| Archive版 | 不能覆盖（包名/签名已变） | — |
| MD3版 | 包名同原版但签名可能不同 | — |

## 兼容性说明

### 书源兼容性

所有 Android 版（基于 legado 3.x）的书源 JSON 格式通用，可互相导入。

**例外：** Tauri 桌面版使用纯 JavaScript 书源体系，与 Android 版书源不兼容。

### 数据迁移兼容性（从原版 3.25 迁移）

| 版本 | 书源 | 缓存数据 | 书架 | 主题 | 备注 |
|------|------|---------|------|------|------|
| LegadoTeam release | 通用 | 通用 | 通用 | 通用 | 最平滑迁移 |
| Sigma/lyc beta | 通用 | 通用 | 通用 | 通用 | 覆盖安装即可 |
| R beta | 通用 | 通用 | 通用 | 部分（主题重做） | 继承自 Archive 线路 |
| Max appLegacy | 通用 | 可能丢失 | 可能丢失 | 通用 | 建议备份后卸载重装 |
| MD3版 | 通用 | 部分 | 分组格式不兼容 | 完全不通用 | 差异最大 |
| Archive版 | 通用 | 不能覆盖安装 | — | — | 包名已变 |
| Tauri桌面版 | 不兼容 | 不兼容 | 不兼容 | — | 完全独立产品 |

---

## 社区链接汇总

### Telegram

| 版本 | 链接 |
|------|------|
| 原版 | [@yueduguanfang](https://t.me/yueduguanfang)（群组）/ [@legado_channels](https://t.me/legado_channels)（频道） |
| Sigma版 | [@readsigma](https://t.me/readsigma) |
| R版 | [@yuedur](https://t.me/yuedur) |
| MD3版 | [@materado](https://t.me/materado) |

### Discord

- 通用 Discord：[discord.gg/VtUfRyzRXn](https://discord.gg/VtUfRyzRXn)

### QQ群（Tauri版）

| 群 | 号码 | 状态 |
|----|------|------|
| 一群 | 645815655 | 已满 |
| 二群 | 949235656 | 已满 |
| 三群 | 1107448928 | 可加入 |

### 其他资源

| 资源 | 链接 |
|------|------|
| 官方帮助文档 | [yuque.com/legado/wiki](https://www.yuque.com/legado/wiki) |
| 书源规则教程 | [mgz0227.github.io/The-tutorial-of-Legado](https://mgz0227.github.io/The-tutorial-of-Legado/) |
| Web端书架 | [gedoor/legado_web_bookshelf](https://github.com/gedoor/legado_web_bookshelf) |
| Web端源编辑 | [gedoor/legado_web_source_editor](https://github.com/gedoor/legado_web_source_editor) |
| LegadoTeam Tauri 文档 | [docs.legadoteam.org](https://docs.legadoteam.org) |
| LegadoTeam 官网 | [legadoteam.org](https://legadoteam.org) |

---

## 推荐选择

### 追求最大兼容性（从原版平滑迁移）

**LegadoTeam release版** > **Sigma/lyc beta版** > **R beta版**

### 追求功能丰富

**Max版** > **R版** > **Sigma版**

### 追求界面美观/现代化

**MD3版** > **Max版**

### 桌面端需求

**LegadoTeam Tauri桌面版**（独立产品，需重新制作/导入书源）

---

## 免责声明

本项目仅汇总公开的开源项目信息，不提供任何书源或内容资源。各版本均为开源项目，请从官方仓库下载，注意安全。使用第三方版本前请做好数据备份。

---

> 最后更新：2026年6月16日
>
> 如有信息错误或遗漏，欢迎提交 Issue 或 PR 补充。
