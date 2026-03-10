# LittleFingers

A fullscreen interactive smash toy for babies and toddlers. Let little hands tap, click, and explore freely — without accidentally closing apps or changing files.

## Features

- **4 Playful Themes** — Confetti, Bubbles, Space, Underwater
- **PIN-Locked Fullscreen** — Kids can't accidentally exit
- **Touch + Keyboard + Mouse** — Works on phones, tablets, laptops, desktops
- **Web Audio Synthesis** — Melodic tones on every tap and keypress
- **Secret Parent Menu** — Long-press top-left corner (2s) or type `parent`
- **Zero Setup** — No install, no account, no tracking

## Usage

Open the site in a browser and tap **"Ready? Let's smash!"** — it goes fullscreen instantly.

### Parent Controls

Access the hidden parent menu by:
- Long-pressing the **top-left corner** for 2 seconds, or
- Typing the word **`parent`** on the keyboard

From the parent menu you can:
- Switch themes
- Toggle sound
- Set a custom PIN (default: `1234`)
- Enable/disable idle demo, reduce motion, full emoji mode

### Exiting Fullscreen

Tap **"Exit Fullscreen"** in the parent menu and enter the PIN.

## Run Locally

No build step needed — it's pure static HTML/CSS/JS.

```bash
git clone git@github.com:Nivs4796/LittleFingers.git
cd LittleFingers
python3 -m http.server 8080
# Open http://localhost:8080
```

## Deploy

| Platform | How |
|----------|-----|
| **GitHub Pages** | Settings → Pages → Deploy from `main` branch |
| **Netlify** | Drag and drop the project folder |
| **Vercel** | `vercel --prod` from the project root |
| **Any static host** | Upload all files preserving directory structure |

## Project Structure

```
LittleFingers/
├── index.html                         # Main app
├── styles.css                         # Stylesheet
├── app.js                             # Canvas + audio engine
├── about/index.html                   # About & privacy
├── baby-keyboard-smash/index.html     # SEO content page
├── toddler-keyboard-smash/index.html  # SEO content page
└── why-babies-love-keyboards/         # SEO content page
```

## Tech Stack

- Vanilla HTML5, CSS3, JavaScript (ES6+)
- HTML5 Canvas API
- Web Audio API
- No frameworks, no dependencies, no build tools
