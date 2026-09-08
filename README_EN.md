> 🌐 Language / 语言: **English** · [中文](README.md)

# Wallpaper Manager

> A Wallpaper Engine auxiliary management tool for managing leftover wallpaper files on the local disk that remain after unsubscribing from the Steam Workshop.

When you **unsubscribe** from a Wallpaper Engine wallpaper on the Steam Workshop, Steam does not always delete the local files immediately — they keep occupying disk space. This tool **scans and lists those wallpapers that are unsubscribed but still left on your local disk**, letting you preview, filter, and clean them up to free space.

<img width="2160" height="1350" alt="图片" src="https://github.com/user-attachments/assets/5573dd8c-804a-45ad-85c9-29deab4ecda2" />

## Features

- 📂 Scan local disk and list wallpapers that are unsubscribed but still present locally
- 👤 Filter by Steam user (user list is loaded automatically after saving config)
- 🔞 Filter by age rating: All / General / Adult
- 🔍 Search by title
- 🖼️ Preview & detail drawer (ID, title, size, rating, status, subscription details)
- ▶ Video files can be played directly using the local player.
- 📂 Open the wallpaper folder / copy its path with one click
- 🗑️ Batch delete selected or all leftover wallpapers to reclaim space (irreversible)
- 📊 Statistics dashboard: subscribed size / releasable space / R18 count
- 🌐 Simplified Chinese / English UI (toggle at the top-right in the app)

## Download & Install

1. Go to the [Releases](https://github.com/Roco65V/WallpaperEngineManage/releases) page.
2. Download `Wallpaper.Manager.Setup.exe` (GitHub displays spaces in the file name as dots).
3. Run the installer and follow the prompts.

## Configuration before first use

On first launch, open **⚙ (Settings)** at the top-right and fill in two paths. Config is saved to `%APPDATA%\Wallpaper Manager\config.json`:

1. **Wallpaper Engine content path**: the Steam Workshop content directory
   - e.g. `D:\Steam\steamapps\workshop\content\431960`
2. **Steam userdata path**: the Steam `userdata` directory
   - e.g. `D:\Steam\userdata`

> These paths vary by your Steam installation; fill them in according to your setup, then click **💾 Save config**. The tool reloads the user list and scans local wallpapers.

## How to use

1. Launch the app. It opens on the **Unsubscribed** list showing leftover wallpaper files on disk.
2. Use the top filter bar to filter by **user** or **rating**; use the search box to find by title.
3. Select the wallpapers to clean up and click **Delete selected**; or click **Delete all** to remove every leftover at once.
   - ⚠️ Deletion is **irreversible** — please confirm before proceeding.
4. Switch to **Subscribed** to view still-subscribed wallpapers; switch to **Statistics** to see disk usage (subscribed size / releasable space / R18 count).
5. Click any wallpaper card to view details, preview, copy path, open folder, or delete.
6. Toggle 中文 / English from the top-right (persisted in config).

## How it works (brief)

- Scans every wallpaper folder (named by `publishedfileid`) under the "Wallpaper Engine content path".
- Reads each Steam user's subscription record at `userdata\<id>\ugc\431960_subscriptions.vdf`.
- A wallpaper that exists on disk but is not "actively subscribed" by any user is flagged as **Unsubscribed (leftover)** and can be safely deleted.

## License

Distributed under the terms in [LICENSE](LICENSE).
