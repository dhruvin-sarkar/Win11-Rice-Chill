<div align="center">
 
<br>
 
```
    .oooooo.                 .                                                          o8o             
   d8P'  `Y8b              .o8                                                          `"'             
  888           .oooo.   .o888oo oo.ooooo.  oo.ooooo.  oooo  oooo   .ooooo.   .ooooo.  oooo  ooo. .oo.  
  888          `P  )88b    888    888' `88b  888' `88b `888  `888  d88' `"Y8 d88' `"Y8 `888  `888P"Y88b 
  888           .oP"888    888    888   888  888   888  888   888  888       888        888   888   888 
  `88b    ooo  d8(  888    888 .  888   888  888   888  888   888  888   .o8 888   .o8  888   888   888 
   `Y8bood8P'  `Y888""8o   "888"  888bod8P'  888bod8P'  `V88V"V8P' `Y8bod8P' `Y8bod8P' o888o o888o o888o
                                  888        888                                                        
                                 o888o      o888o                                                          
```
 
### a catppuccin mocha windows 11 rice
 
<br>

![Windows 11](https://img.shields.io/badge/Windows%2011-cba6f7?style=for-the-badge&logo=windows11&logoColor=1e1e2e)
![License](https://img.shields.io/badge/License-Apache%202.0-cba6f7?style=for-the-badge&labelColor=1e1e2e)
![Stars](https://img.shields.io/github/stars/dhruvin-sarkar/Win11-Rice-Catppuccin?style=for-the-badge&color=cba6f7&labelColor=1e1e2e)

<br>

</div>

---

> **Catppuccin** is a Windows 11 rice built around niivu's Catppuccin Mocha theme, patched with SecureUXTheme.Catppuccin ports across every app that supports them.

---

## Screenshots

<div align="center">

| Desktop | Terminal |
|:---:|:---:|
| `screenshot here` | `screenshot here` |

| Nilesoft Shell | Fastfetch |
|:---:|:---:|
| `screenshot here` | `screenshot here` |

</div>

---

## Software Stack

| Category | Tool |
|---|---|
| **OS** | Windows 11 |
| **Tiling WM** | [Komorebi](https://github.com/LGUG2Z/komorebi) |
| **Hotkey Daemon** | [WHKD](https://github.com/LGUG2Z/whkd) |
| **Status Bar** | [YASB](https://github.com/amnweb/yasb) |
| **Shell Theme** | [Niivu's Catppuccin for Windows 11](https://www.deviantart.com/niivu/art/Catppuccin-for-Windows-11-1076249390) |
| **Theme Patcher** | [SecureUXTheme](https://github.com/namazso/SecureUxTheme) |
| **Icon Pack** | Catppuccin Teal via [Windhawk Resource Redirect](https://windhawk.net/mods/icon-resource-redirect) |
| **Context Menu** | [Nilesoft Shell](https://nilesoft.org/) |
| **Window Tweaks** | [Windhawk](https://windhawk.net/) |
| **Hotkeys / Macros** | [AutoHotKey v2](https://www.autohotkey.com/) |
| **Fetch** | [Fastfetch](https://github.com/fastfetch-cli/fastfetch) |
| **Shell Prompt** | [Oh My Posh](https://ohmyposh.dev/) |
| **App Launcher** | [Flow Launcher](https://www.flowlauncher.com/) |
| **Browser Themes** | [Stylus](https://github.com/openstyles/stylus) |
| **New Tab Page** | [mtab](https://github.com/maxhu08/mtab) (Zen Browser) |
| **App Theming** | [Catppuccin Ports](https://catppuccin.com/ports) |
| **Wallpapers** | Various — included in `Backgrnds/` |
| **Font** | [JetBrainsMono Nerd Font](https://www.nerdfonts.com/font-downloads) |

---

## Fonts

Install these before setting anything up -- icons and prompt glyphs depend on them.

- **[JetBrainsMono Nerd Font](https://www.nerdfonts.com/font-downloads)** -- used everywhere (terminal, YASB, Oh My Posh)
- **[JetBrains Mono](https://www.jetbrains.com/lp/mono/)** -- non-Nerd variant for editors if preferred

After downloading, right-click the `.ttf` files and select **Install for all users**.

---

## Installation

> [!NOTE]
> **Back up your existing configs before copying anything.** All destination paths point to live config locations. If you already use any of these tools, manually merge rather than overwrite.

> [!NOTE]
> Each section shows: `repo folder/file` -> `where to put it on your system`

---

### Windows Theme (SecureUXTheme + Niivu's Catppuccin)

> [!NOTE]
> This is the most involved step. Read it carefully before proceeding. Create a System Restore Point first.

**Step 1 -- Patch Windows to allow third-party themes**

Download SecureUXTheme from [github.com/namazso/SecureUxTheme](https://github.com/namazso/SecureUxTheme/releases).

Run it as Administrator. Click **Install** (enable "Hook LogonUI" if you want lock screen consistency). Reboot.

> [!NOTE]
> Your antivirus may flag SecureUXTheme. This is a false positive caused by the elevated, unsigned executable. The source code is fully public. The developer submits releases to Microsoft for analysis before each release.

**Step 2 -- Install the theme**

Download niivu's Catppuccin for Windows 11 from [DeviantArt](https://www.deviantart.com/niivu/art/Catppuccin-for-Windows-11-1076249390).

Copy the `.theme` file and the accompanying theme folder (same name as the theme) to:

```
C:\Windows\Resources\Themes\
```

> [!NOTE]
> Do not double-click the `.theme` file. Custom themes must be placed in the Themes folder manually and then applied through SecureUXTheme.

**Step 3 -- Apply the theme**

Open SecureUXTheme as Administrator. Find your theme in the list. Click **Patch and Apply**. The desktop will refresh.

**Step 4 -- Apply custom modifications**

The theme folder from this repo includes settings from niivu's installation guide (extra info section). This covers:

- Caption buttons removed (minimize, maximize, close) -- this is the custom version
- OldNewExplorer settings for Explorer styling

Follow niivu's [installation guide](https://www.deviantart.com/niivu/art/How-to-install-Windows-10-or-11-Themes-708835586) for the full extra-info section, including OldNewExplorer configuration.

---

### Komorebi + WHKD *(Tiling WM)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://youtube.com/@LGUG2Z)

Install Komorebi: [github.com/LGUG2Z/komorebi/releases](https://github.com/LGUG2Z/komorebi/releases)

Install WHKD: [github.com/LGUG2Z/whkd/releases](https://github.com/LGUG2Z/whkd/releases)

```
komorebi.json  →  %USERPROFILE%\komorebi.json
whkdrc         →  %USERPROFILE%\.config\whkdrc
```

Start with:
```powershell
komorebic start --whkd
```

To autostart, add the above command to your PowerShell profile or place a startup script in `shell:startup`.

---

### YASB *(Status Bar)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=yasb+windows+status+bar+setup)

Install: [github.com/amnweb/yasb/releases](https://github.com/amnweb/yasb/releases)

```
YASB/config.yaml  →  %USERPROFILE%\.config\yasb\config.yaml
YASB/styles.css   →  %USERPROFILE%\.config\yasb\styles.css
```

> [!NOTE]
> Requires a Nerd Font for icons to render correctly.

Restart YASB after copying. To autostart, place a shortcut to `yasb.exe` in `shell:startup`.

---

### Nilesoft Shell *(Context Menu)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=nilesoft+shell+context+menu+windows+11+setup)

Install:
```powershell
winget install -e --id Nilesoft.Shell
```

Or download from [nilesoft.org](https://nilesoft.org/).

```
nilesoft-shell/shell.nss  →  C:\Program Files\Nilesoft Shell\shell.nss
```

After copying, reload with `Ctrl+Right-click` on the desktop.

> [!NOTE]
> Copying to `Program Files` requires Administrator permissions. Open an elevated terminal to copy the file manually if needed.

---

### Windhawk *(Window Tweaks + Icon Pack)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=windhawk+windows+11+taskbar+setup+tutorial)

Install: [windhawk.net](https://windhawk.net/)

```
windhawk/  →  reference folder -- see note below
```

> [!NOTE]
> Windhawk stores mod settings in the Windows registry, not as portable files. The `windhawk/` folder documents the mods used and their settings as reference. Install each mod from the Windhawk UI and configure them manually using the values shown.

**Mods used in this rice:**

- **Taskbar Styler** -- custom taskbar appearance
- **Start Menu Styler** -- custom start menu appearance
- **Resource Redirect (Icon Resource Redirect)** -- applies the Catppuccin Teal icon pack

For the icon pack, install the Resource Redirect mod, then download [niivu's Catppuccin icon theme for Windhawk](https://github.com/niivu/resource-redirect-icon-themes) and point the mod's config to the icon folder.

---

### AutoHotKey *(Hotkeys and Macros)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=autohotkey+v2+windows+setup+tutorial)

Install AutoHotKey v2: [autohotkey.com](https://www.autohotkey.com/)

```
ahk/  →  place .ahk files anywhere, then create a shortcut to each in shell:startup
```

To autostart scripts on login:

1. Press `Win+R` and type `shell:startup`
2. Create a shortcut to your `.ahk` file(s) and place it in the folder that opens

To run immediately, just double-click any `.ahk` file.

---

### Fastfetch

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=fastfetch+windows+setup+tutorial)

Install:
```powershell
winget install fastfetch-cli.fastfetch
```

```
fastfetch/  →  %USERPROFILE%\.config\fastfetch\
```

Run with `fastfetch` in your terminal.

---

### Oh My Posh *(Shell Prompt)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=oh+my+posh+windows+terminal+catppuccin+setup)

Install:
```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```

```
oh-my-posh/<theme>.omp.json                       →  %USERPROFILE%\<theme>.omp.json
oh-my-posh/Microsoft.PowerShell_profile.ps1       →  $PROFILE
```

To find your profile path:
```powershell
echo $PROFILE
```

> [!NOTE]
> The PowerShell profile already contains the `oh-my-posh init` line pointing to the theme file. The theme is based on the Zen OMP config -- make sure the path in `$PROFILE` matches where you placed the `.omp.json`.

---

### Stylus *(Browser Website Themes)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=stylus+browser+extension+custom+css+theme+catppuccin)

Install Stylus for your browser:

- [Chrome / Chromium](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)
- [Firefox / Zen](https://addons.mozilla.org/en-US/firefox/addon/styl-us/)

```
stylus/  →  import via Stylus extension backup
```

To import:
1. Open the Stylus extension options (click the icon, then the cog)
2. Go to **Backup** and select **Import**
3. Point it at the backup file in the `stylus/` folder

Alternatively, each `.user.css` file in the folder can be dragged directly into the Stylus management page to install individual styles.

> [!NOTE]
> Most of the Catppuccin web themes here are ports from [userstyles.world](https://userstyles.world/). You can also browse and install them directly from there if you prefer not to use the backup.

---

### Flow Launcher *(App Launcher)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=flow+launcher+windows+catppuccin+theme+setup)

Install: [flowlauncher.com](https://www.flowlauncher.com/)

> [!NOTE]
> Flow Launcher config is not included in this repo. Install it, then apply a Catppuccin theme from within Flow's settings under **Themes**. The Catppuccin theme can be found on [userstyles.world](https://userstyles.world/) or by searching "Catppuccin" inside the Flow Launcher theme browser.

---

### mtab *(New Tab Page for Zen Browser)*

[![Tutorial](https://img.shields.io/badge/YouTube-Tutorial-cba6f7?style=flat-square&logo=youtube&logoColor=1e1e2e)](https://www.youtube.com/results?search_query=mtab+new+tab+page+browser+extension+setup)

Install mtab for Zen / Firefox: [addons.mozilla.org](https://addons.mozilla.org/en-US/firefox/addon/mtab/)

Or for Chromium: [Chrome Web Store](https://chromewebstore.google.com/detail/mtab/fdaphilojaklgkoocegabckfanjoacjg)

> [!NOTE]
> mtab supports quick config sharing natively. A config export file is included in the repo. To import: open a new tab, click the mtab settings gear, go to **Import/Export**, and paste or load the config file.

---

### Catppuccin Ports *(Other Apps)*

All other app themes come from the official [Catppuccin Ports](https://catppuccin.com/ports) list. Visit the site, find the port for whichever app you use, and follow its individual install instructions.

Popular ports relevant to this setup:

| App | Port |
|---|---|
| VSCode | [catppuccin/vscode](https://github.com/catppuccin/vscode) |
| Discord | [catppuccin/discord](https://github.com/catppuccin/discord) |
| Firefox | [catppuccin/firefox](https://github.com/catppuccin/firefox) |
| Obsidian | [catppuccin/obsidian](https://github.com/catppuccin/obsidian) |
| Spotify (Spicetify) | [catppuccin/spicetify](https://github.com/catppuccin/spicetify) |

---

### Wallpapers

No install needed -- the `Backgrnds/` folder contains the wallpapers used in this rice.

Sources include various wallpaper repos and subreddits (credits where identifiable are listed in the folder).

Right-click any image and select **Set as desktop background**, or use Windows Settings > Personalization > Background.

---

## Repo Structure

```
Win11-Rice-Catppuccin/
├── Backgrnds/            # Wallpapers
├── YASB/                 # Status bar config
├── ahk/                  # AutoHotKey scripts
├── fastfetch/            # Fetch tool config
├── nilesoft-shell/       # Context menu config (shell.nss)
├── oh-my-posh/           # Shell prompt theme + PowerShell profile
├── stylus/               # Browser CSS themes backup/files
├── windhawk/             # Windhawk mod settings reference
├── komorebi.json         # Tiling WM config
└── whkdrc                # WHKD hotkey daemon config
```

---

## Notes

- **Caption buttons removed** -- the theme applied here is a custom edit of niivu's Catppuccin that hides the minimize, maximize, and close window buttons. This is intentional. If you want them back, download the standard version from niivu's DeviantArt page and apply that instead.
- **Windhawk settings** -- these live in the Windows registry and cannot be portably shared as files. The `windhawk/` folder contains a documented reference of which mods are active and the settings used for each.
- **OldNewExplorer** -- referenced in niivu's installation guide extra-info section. Used here to adjust Explorer UI elements that the theme targets. Follow niivu's guide for the exact settings.
- **Screen resolution** -- this setup was configured on a *[your resolution]* display. YASB widget sizes and some theme elements may need adjustment on other resolutions.
- **Also check out** -- [Ash](https://github.com/dhruvin-sarkar/Win11-Rice-Ash) (grey), [Monochrome](https://github.com/dhruvin-sarkar/Win11-Rice-Monochrome) (black and white), and [Evergreen](https://github.com/dhruvin-sarkar/Win11-Rice-Evergreen) (forest green) for other rices in this series.

---

## Acknowledgements

- [niivu](https://www.deviantart.com/niivu) for the Catppuccin Windows theme and the comprehensive installation guide
- [Catppuccin](https://catppuccin.com/) for the colour palette and all the ports
- [LGUG2Z](https://github.com/LGUG2Z) for Komorebi and WHKD
- [r/unixporn](https://reddit.com/r/unixporn) and [r/desktops](https://reddit.com/r/desktops) for the rice culture
- [winthemers/wiki](https://github.com/winthemers/wiki) for the SecureUXTheme guide

---

<div align="center">

<br>

*if this rice helped you, a star is appreciated*

<br>

</div>
