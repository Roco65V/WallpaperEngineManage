# WallpaperEngineManage

> 🇨🇳 中文 ｜ 🇺🇸 [English](#english)

Wallpaper Engine 辅助管理工具，用于展示与管理 Steam 创意工坊中已取消订阅但仍在本地磁盘残留的壁纸文件。
*A Wallpaper Engine auxiliary management tool for managing leftover wallpaper files on the local disk that remain after unsubscribing from the Steam Workshop.*

---

## 🇨🇳 中文说明

<details open>
<summary><b>点击展开 / 收起中文说明</b></summary>

### 简介

当你在 Steam 创意工坊**取消订阅**某个 Wallpaper Engine 壁纸后，Steam 有时并不会立即删除本地文件，这些壁纸会一直占用磁盘空间。本工具用于**扫描并列出这些「已取消订阅但仍残留在本地」的壁纸**，帮助你预览、筛选并清理它们，释放磁盘空间。

### 功能特性

- 📂 扫描本地磁盘，列出已取消订阅但仍在本地的壁纸
- 👤 按 Steam 用户筛选（保存配置后自动加载用户列表）
- 🔞 按年龄分级筛选：全部 / 大众级 / 成人（Adult）
- 🔍 按标题搜索
- 🖼️ 预览图 / 详情抽屉（ID、标题、大小、状态、订阅详情）
- 📂 一键打开壁纸所在文件夹、复制路径
- 🗑️ 批量删除选中或全部残留壁纸，释放空间
- 📊 统计看板（已订阅 / 未订阅 / 可释放空间）
- 🌐 简体中文 / English 双语界面（安装时选择语言）

### 下载与安装

1. 前往 [Releases](https://github.com/Roco65V/WallpaperEngineManage/releases) 页面。
2. 下载 `Wallpaper Manager Setup.exe`。
3. 运行安装程序，按提示完成安装（安装过程中可选择界面语言）。

### 使用方法

1. 启动应用，点击右上角 **⚙（设置）** 或导航栏 **设置**。
2. 在设置中填写两个路径（首次使用必须填写，工具不会自动探测）：
   - **Wallpaper Engine 内容路径**：Steam 创意工坊内容目录
     - 例如：`D:\Steam\steamapps\workshop\content\431960`
   - **Steam 用户数据路径**：Steam 的 `userdata` 目录
     - 例如：`D:\Steam\userdata`
3. （可选）设置「每页显示数量」。
4. 点击 **💾 保存配置**。保存后工具会重新加载用户列表并扫描本地壁纸。
5. 切换到 **未订阅** 标签页，浏览所有残留壁纸；可使用顶部搜索框、用户筛选、分级筛选缩小范围。
6. 点击卡片查看预览与详情；勾选后点击 **删除选中** 或 **删除全部** 清理文件、释放空间。
   - ⚠️ 删除操作**不可撤销**，请确认后再执行。

### 数据存储

- 配置保存在应用用户数据目录的 `config.json`。
- 安装器语言保存在 `install-locale.json`，每次启动以安装时选择的语言为准。

### 从源码构建（可选）

```bash
npm install
npm run build
# 产物位于 release/Wallpaper Manager Setup.exe
```

</details>

---

## 🇺🇸 English

<details>
<summary><b>Click to expand / collapse English</b></summary>

### Overview

When you **unsubscribe** from a Wallpaper Engine wallpaper on the Steam Workshop, Steam does not always delete the local files immediately — they keep occupying disk space. This tool **scans and lists those wallpapers that are unsubscribed but still left on your local disk**, letting you preview, filter, and clean them up to free space.

### Features

- 📂 Scan local disk and list wallpapers that are unsubscribed but still present locally
- 👤 Filter by Steam user (user list is loaded automatically after saving config)
- 🔞 Filter by age rating: All / General / Adult
- 🔍 Search by title
- 🖼️ Preview & detail drawer (ID, title, size, status, subscription details)
- 📂 Open the wallpaper folder / copy its path with one click
- 🗑️ Batch delete selected or all leftover wallpapers to reclaim space
- 📊 Statistics dashboard (subscribed / unsubscribed / releasable space)
- 🌐 Simplified Chinese / English UI (choose language at install time)

### Download & Install

1. Go to the [Releases](https://github.com/Roco65V/WallpaperEngineManage/releases) page.
2. Download `Wallpaper Manager Setup.exe`.
3. Run the installer and follow the prompts (you can choose the UI language during installation).

### How to use

1. Launch the app and open **⚙ (Settings)** at the top-right, or the **Settings** nav item.
2. Fill in the two paths (required on first use; the tool does **not** auto-detect them):
   - **Wallpaper Engine content path**: the Steam Workshop content directory
     - e.g. `D:\Steam\steamapps\workshop\content\431960`
   - **Steam userdata path**: the Steam `userdata` directory
     - e.g. `D:\Steam\userdata`
3. (Optional) Set **items per page**.
4. Click **💾 Save settings**. The tool reloads the user list and scans local wallpapers.
5. Switch to the **Unsubscribed** tab to browse all leftover wallpapers; use the search box, user filter, and rating filter at the top to narrow down.
6. Click a card to view preview & details; select items and click **Delete selected** or **Delete all** to clean up files and free space.
   - ⚠️ Deletion is **irreversible** — please confirm before proceeding.

### Data storage

- Config is saved to `config.json` in the app's user data directory.
- The installer language is saved to `install-locale.json`; the app starts in the language chosen at install time.

### Build from source (optional)

```bash
npm install
npm run build
# Output: release/Wallpaper Manager Setup.exe
```

</details>

---

## 📄 License

See [LICENSE](LICENSE).
