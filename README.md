# 🎮 JaraServices – Free Loading Screen

A **modern and fully customizable FiveM loading screen**, designed for RP servers that want a professional look with music, rules, and server info.

> 💜 Developed by **Jaramiyo** – [JaraServices.com](https://www.jaraservices.com)

---

## ✨ Features

* 🖼️ **Fully configurable** via `config.json`
* 🎧 Built-in **music player** with custom track list
* 📱 **Social links cards** (Discord, Instagram, TikTok, YouTube, etc.)
* ⚙️ **Dynamic rules panel** and **team section**
* 🖥️ **Gallery slideshow** for vehicle or server showcase images
* 🎮 **Keyboard shortcuts** panel (configurable keys for RP servers)
* 💡 **Auto color theme** (set your brand color with one value)

---

## 📦 Installation

1. Drop the folder into your FiveM resources:

   ```
   resources/[jaraservices]/js_loadscreen
   ```

2. Add it to your `server.cfg`:

   ```cfg
   ensure js_loadscreen
   ```

3. Done!
   The loading screen will automatically appear when players join your server.

---

## ⚙️ Configuration

All customization is handled inside **`config.json`**
Below is a breakdown of every section:

---

### 🎨 Theme

```json
"selectedColor": "#ff007b",
"backgroundImage": "./assets/png/supra1.png",
"videoUrl": ""
```

* `selectedColor`: Accent color for buttons, sliders, and highlights
* `backgroundImage`: Path to background image (PNG/JPG)
* `videoUrl`: Optional background video (YouTube or hosted .mp4)

---

### 🖋️ Branding

```json
"watermark": {
  "label": { "text": "Island RP", "colorWordCount": 2 },
  "subHeading": "Loading Screen",
  "logo": "./assets/png/logo.png"
}
```

* `text`: Server name
* `colorWordCount`: How many words from the name use the accent color
* `subHeading`: Subtitle under your logo
* `logo`: Image path for your server logo

---

### 🌐 Social Headers

Each social card can be enabled/disabled individually:

```json
{
  "type": "discord",
  "cardLabel": "Discord Server",
  "cardInfo": "Join the discord to keep up with the latest on the FiveM server!",
  "link": "https://discord.gg/KKqZkg8HJY",
  "enabled": true
}
```

Available types:
🟣 `discord`, 🟠 `instagram`, 🔵 `telegram`, 🔴 `youtube`, 🎵 `tiktok`

---

### 📜 Rules

```json
"rules": [
  "No griefing or trolling other players.",
  "Respect all admins and staff decisions.",
  "No hacking, exploiting, or modding in unfair ways."
]
```

Displayed in the right-hand **Server Rules** panel.

---

### 👥 Team Members

```json
"teamMembers": [
  { "name": "GucciFlipFlops", "role": "Head Developer", "discord": "pakinextdoor", "image": "./assets/png/fakalheadshot.png" }
]
```

Each entry shows member info and avatar in the **staff section**.

---

### 🖼️ Gallery

```json
"gallery": [
  { "path": "./assets/jpg/supra1.jpg" },
  { "path": "./assets/png/bluebmw.png" }
]
```

Rotates background images for a cinematic effect.
Supports `.jpg` and `.png`.

---

### 🎹 Keyboard Shortcuts

```json
{
  "key": "B",
  "onFoot": "Point",
  "inCar": "Put on seatbelt"
}
```

* Displays common controls for new players.
* Add/remove keys freely to match your server setup.

---

### 🎵 Music Player

```json
{
  "path": "./assets/mp3/gta.mp3",
  "title": "GTA",
  "artist": "Future, Metro Boomin",
  "image": null
}
```

* Add as many songs as you like (MP3 format).
* Optional image per song.
* Volume controlled by `defaultVolume` (0–100).

---

## 🖌️ Customization Tips

* For best results, keep all images below **2MB** to avoid long load times.
* You can use **.mp4** background videos (hosted locally or via URL).
* Change `selectedColor` to match your brand (e.g., purple `#7a00ff` or gold `#f1c40f`).

---

## 📜 License

**MIT License** — Free to use, modify, and redistribute.
Please keep credits to **JaraServices**.

---

## 💬 Support & Links

* 🌐 Website: [https://www.jaraservices.com/](https://www.jaraservices.com/)
* 💬 Discord: [https://discord.gg/KKqZkg8HJY](https://discord.gg/KKqZkg8HJY)

> Free release by **JaraServices** – professional scripts, tools, and designs for FiveM & RP servers.
