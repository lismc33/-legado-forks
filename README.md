
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

**最近更新：**

| 版本号 | 日期 | 类型 | 更新内容 |
|--------|------|------|---------|
| 3.26.032122 | 2026-03-21 | Pre-release | 优化发现结果无障碍；支持视频播放简介的web渲染；低安卓上图标圆角 |
| 3.26.030717 | 2026-03-07 | Stable | 优化代码，修复问题 |
| 3.26.030223 | 2026-03-02 | Stable | 视频悬浮窗播放系统媒体通知；净化规则js支持java.log；代码编辑器搜索替换支持$符号；优化书架滚动位置记忆；自动检查app更新 |

**版本类型与 APK 分发：**

| APK 文件名格式 | 包名 | 说明 |
|---------------|------|------|
| `legado_beta_*_release.apk` | `io.legado.app`（同原版） | 覆盖原版安装，更新频繁 |
| `legado_plus_*_releaseS.apk` | 共存包名 | 不覆盖原版，稳定阶段更新 |

**社区：**

| 平台 | 链接 |
|------|------|
| Telegram | [@readsigma](https://t.me/readsigma) |
| Discord | [加入](https://discord.gg/VtUfRyzRXn) |
| 微信公众号 | legado_plus |

**下载：** [GitHub Releases](https://github.com/Luoyacheng/legado/releases) / [Gitee Releases](https://gitee.com/lyc486/legado/releases)

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

**最近更新：**

| 版本号 | 日期 | 类型 | 更新内容 |
|--------|------|------|---------|
| 3.26.060703 | 2026-06-06 | Stable | 提升发现页封面缓存命中率；调整音频/视频缓存存储位置；优化视频加载与播放；修复书架默认分组无法重命名 |
| 3.26.060303 | 2026-06-02 | Stable | 修复TTS异常停顿；视频无缝切换；新增缓存统计功能；备份与恢复项目选择功能 |
| 3.26.052908 | 2026-05-29 | Stable | 导出书籍自动移除段评；AudioBook新增快进/快退；优化TTS体验；修复主题编辑图片问题 |

**APK 分发：**

| APK 文件名格式 | 说明 |
|---------------|------|
| `legado_app_3.26.*_*.apk` | 单一 APK，无 beta/plus 区分 |

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

**最近更新（主仓库 youfengknight）：**

| 版本号 | 日期 | 类型 | 更新内容 |
|--------|------|------|---------|
| beta-3.26.061408 | 2026-06-14 | Pre-release | 修复底栏编辑界面无法滚动；高亮规则编辑界面开关颜色修复 |
| beta-3.26.060522 | 2026-06-05 | Pre-release | 增加java/Android API文档；帮助文档管理器支持自定义文档；修复复用WebView搜索页空白 |

**最近更新（复刻仓库 Suml-1，更新更频繁）：**

| 版本号 | 日期 | 类型 | 更新内容 |
|--------|------|------|---------|
| beta-3.26.061522 | 2026-06-15 | Pre-release | 修复列表布局下作者/当前章节/最新章节行间距不一 |
| beta-3.26.061513 | 2026-06-15 | Pre-release | 无底栏管理；修复屏蔽规则持久化及订阅源崩溃；修复横竖屏切换章节内容显示不全 |
| beta-3.26.061500 | 2026-06-14 | Pre-release | 书架布局新增书籍外边框显示开关并优化列表间距 |

**版本类型与 APK 分发：**

| APK 文件名格式 | 包名 | 说明 |
|---------------|------|------|
| `legado_beta_*_release.apk` | `io.legado.app.yuedu` | 主 Max 版，共存安装 |
| `legado_compat_*_legacy.apk` | `io.legado.app`（同原版） | 兼容版，可覆盖原版安装 |
| `legado_plus_*_releaseS.apk` | `io.legado.app.yuedu.a` | 另一个共存包名 |

> 复刻版 Suml-1/Legado_Max 的 APK 分发格式完全相同，版本号更新更频繁（如 `beta-3.26.061522`）。

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

**APK 分发（按 CPU 架构）：**

| APK 文件名格式 | 说明 |
|---------------|------|
| `legado-3.26.*-beta.*-arm64-v8a.apk` | 64 位设备（推荐大多数现代手机） |
| `legado-3.26.*-beta.*-armeabi-v7a.apk` | 32 位设备 |
| `legado-3.26.*-beta.*-noR8-arm64-v8a.apk` | 64 位无混淆版（用于崩溃调试） |
| `legado-3.26.*-beta.*-noR8-armeabi-v7a.apk` | 32 位无混淆版（用于崩溃调试） |
| `legado-3.26.*-beta.*-noR8.apk` | 通用无混淆版 |
| `legado-3.26.*-beta.*.apk` | 通用版 |

> **noR8** 变体关闭了代码混淆与压缩，若遇到崩溃问题请使用它收集日志反馈给开发者。

**社区：**

| 平台 | 链接 |
|------|------|
| Telegram | [Legado with MD3](https://t.me/materado) |
| Telegram 反馈群 | [加入](https://t.me/+Yn1_v5PZqddmMjQ1) |

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

**版本类型与 APK 分发：**

| APK 文件名格式 | 包名 | 说明 |
|---------------|------|------|
| `legado_app_*_release.apk` | `io.legado.app`（同原版） | 覆盖原版安装 |
| `legado_app_*_releaseA.apk` | `com.legado.app.releaseA` | 共存版，不覆盖原版 |

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

| 版本 | 覆盖原版 APK | 包名 | 共存 APK | 共存包名 |
|------|-------------|------|---------|---------|
| 原版 | — | `io.legado.app` | — | — |
| Sigma/lyc | `legado_beta_*_release.apk` | `io.legado.app` | `legado_plus_*_releaseS.apk` | 共存包名 |
| R版 | `legado_app_3.26.*_*.apk` | 单一 APK | — | — |
| Max主仓库 | `legado_compat_*_legacy.apk` | `io.legado.app` | `legado_beta_*_release.apk` / `legado_plus_*_releaseS.apk` | `io.legado.app.yuedu` / `io.legado.app.yuedu.a` |
| Max复刻 | `legado_compat_*_legacy.apk` | `io.legado.app` | `legado_beta_*_release.apk` / `legado_plus_*_releaseS.apk` | `io.legado.app.yuedu` / `io.legado.app.yuedu.a` |
| LegadoTeam | `legado_app_*_release.apk` | `io.legado.app` | `legado_app_*_releaseA.apk` | `com.legado.app.releaseA` |
| Archive版 | 不能覆盖 | 包名/签名已变 | — | — |
| MD3版 | 按 CPU 架构分包 | 包名同原版但签名可能不同 | — | — |

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
