# Firefox Monet
<img width="650" height="500" alt="Screenshot_2026-04-09_17-19-14(1)" src="https://github.com/user-attachments/assets/7bb875ea-4b77-41b7-b1ae-9dfe097f5706" />

A minimal dark Firefox theme that dynamically colors the interface using the system's accent color (works on Windows, Linux and probably MacOS) while maintaining the browser's default layout and behavior.

## Installation

1. Go to `about:config` and set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`
2. Find your profile folder via `about:profiles`
3. Create a `chrome` folder in your profile directory
4. Save `userChrome.css` & `userContent.css` in the chrome folder
5. Restart Firefox

## Simpler version
### Windows
```bash
cd $env:APPDATA\Mozilla\Firefox\profiles\*.release

mkdir chrome

cd chrome

wget https://raw.githubusercontent.com/zachvlat/firefox-monet/refs/heads/main/chrome/userChrome.css -O userChrome.css

wget https://raw.githubusercontent.com/zachvlat/firefox-monet/refs/heads/main/chrome/userContent.css -O userContent
```
### Linux (Flatpak)
```bash
cd ./var/org.mozilla.firefox/config/mozilla/profiles

for /d %i in (*release*) do mkdir "%i\chrome"

for /d %i in (*release*) do wget -O "%i\chrome\userChrome.css" https://raw.githubusercontent.com/zachvlat/firefox-monet/refs/heads/main/chrome/userChrome.css

for /d %i in (*release*) do wget -O "%i\chrome\userContent.css" https://raw.githubusercontent.com/zachvlat/firefox-monet/refs/heads/main/chrome/userContent.css

```

## Examples

<img width="1280" height="720" alt="2025-11-25_14-09" src="/Screenshot_2026-04-09_17-19-14.png" />
<img width="1280" height="720" alt="2025-11-25_14-09" src="/Screenshot_2026-04-09_17-19-51.png" />
<img width="1280" height="720" alt="2025-11-25_14-09" src="/Screenshot_2026-04-09_17-20-41.png" />

## Thanks

Special thanks to MrOtherGuy's [Firefox CSS Hacks](https://github.com/MrOtherGuy/firefox-csshacks/) which is a great material for creating themes on Firefox.
