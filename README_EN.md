> 🌐 Language / 语言: **English** · [中文](README.md)

# Wallpaper Manager

> A Wallpaper Engine auxiliary management tool for managing leftover wallpaper files on the local disk that remain after unsubscribing from the Steam Workshop.

When you **unsubscribe** from a Wallpaper Engine wallpaper on the Steam Workshop, Steam does not always delete the local files immediately — they keep occupying disk space. This tool **scans and lists those wallpapers that are unsubscribed but still left on your local disk**, letting you preview, filter, and clean them up to free space.

<img width="2160" height="1350" alt="screenshot" src="https://github.com/user-attachments/assets/3c91ef5e-c778-4454-85d8-d1747f6213b3" />


<img width="2160" height="1350" alt="screenshot" src="https://github.com/user-attachments/assets/c3b9459e-d590-474c-848a-e5f6a651ff68" />


## Features

- 📂 Scan local disk and list wallpapers that are unsubscribed but still present locally
- 👤 Filter by Steam user (user list is loaded automatically after saving config)
- 🔞 Filter by age rating: All / General / Adult
- 🔍 Search by title
- 🖼️ Preview & detail drawer (ID, title, size, rating, status, subscription details)
- ▶ Video files can be played directly using the local player
- 📂 Open the wallpaper folder / copy its path with one click
- 🗑️ Batch delete selected or all leftover wallpapers to reclaim space (irreversible)
- 📊 Statistics dashboard: subscribed size / releasable space / R18 count
- 🔄 Switch Steam account: go offline / delete the old account's subscription file / go back online to stop Wallpaper Engine from auto-downloading other accounts' wallpapers when switching
- 🌐 Simplified Chinese / English UI (toggle at the top-right in the app)

## Download & Install

1. Go to the [Releases](https://github.com/Roco65V/WallpaperEngineManage/releases) page.
2. Download `Wallpaper.Manager.Setup.exe` (GitHub displays spaces in the file name as dots).
3. Run the installer and follow the prompts.

## Configuration before first use

1. **Steam install directory**:
   - e.g. `D:\Steam`
   Fill in the following paths manually when auto-detection fails.
2. **Wallpaper Engine content path**: the Workshop content path
   - e.g. `D:\Steam\steamapps\workshop\content\431960`
3. **Steam userdata path**: Steam's `userdata` directory
   - e.g. `D:\Steam\userdata`
4. **Wallpaper Engine install path**: the `bin` directory under the Wallpaper Engine install path
   - e.g. `D:\Steam\steamapps\common\wallpaper_engine\bin`

> The paths vary depending on where Steam is installed on your machine. Fill them in according to your actual setup, then click **💾 Save config**. After saving, the tool reloads the user list and scans local wallpapers.

## How to use

1. Launch the app. It opens on the leftover wallpaper files on disk; for video files, click the play button on the card to invoke your system's default player.
2. Use the top filter bar to filter by **user** or **rating**; use the search box to find by title.
3. Select the wallpapers to clean up and click **Delete selected**; or click **Delete all** to remove every leftover at once. (For still-subscribed wallpapers, go to Wallpaper Engine to unsubscribe first.)
   - ⚠️ Deletion is **irreversible** — please confirm before proceeding.
4. Switch to **Subscribed** to view still-subscribed wallpapers; switch to **Statistics** to see disk usage (subscribed size / releasable space / R18 count).
5. Click any wallpaper card to view details, preview, copy path, open folder, or delete.
6. Toggle 中文 / English from the top-right (persisted in config).

## Switch Steam Account

The "Switch Account" item in the sidebar (below "Statistics") lets you **stop Wallpaper Engine from auto-downloading other accounts' wallpapers when switching between multiple Steam accounts**.

If more than one Steam account has been used on the same PC, Wallpaper Engine auto-downloads the new account's subscribed wallpapers after a switch — filling the disk with wallpapers from different accounts. This module avoids that with "go offline → clean subscriptions → go back online":

1. Go offline before switching accounts.
3. After switching back, pick the old account to clean up from the "Select user" dropdown and view the status of its subscription file.
4. Click **Delete subscription file** to remove that account's subscription record (confirmation is required before deletion).
5. Once cleanup is done, switch Wallpaper Engine back **online**.

> Recommended flow: **go offline first → delete the old account's subscription file → go back online**. This prevents auto-downloading other accounts' wallpapers on switch, and stops the old account's subscriptions from being restored.

## License

Distributed under the terms in [LICENSE](LICENSE).
