# How to setup oh-my-posh
1. Install oh-my-posh
```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```
2. Install NerdFonts (by [this guide](https://ohmyposh.dev/docs/installation/fonts))
3. Install CLink for oh-my-posh (for cmd.exe) (by [this guide](https://github.com/TheEnderOfficial/dotfiles/blob/main/clink/oh-my-posh.lua))
4. Setup oh-my-posh for powershell.exe
4.1 Create profile for powershell
```powershell
New-Item -Path $PROFILE -Type File -Force
```
4.2 Open this profile in notepad
```powershell
notepad $PROFILE
```
4.3 Paste this to profile file and save
```powershell
oh-my-posh init pwsh --config "$env:POSH_THEMES_PATH/catppuccin.omp.json" | Invoke-Expression
```
