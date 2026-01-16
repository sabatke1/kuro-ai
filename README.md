# Kuro AI

A minimal 3D AI assistant with voice interaction.

## Features

- 3D VRM model with animations
- Voice input (microphone)
- Voice output (text-to-speech)  
- Powered by Gemini AI (free)

## Setup

1. Download/clone this repository
2. Get a free API key at [aistudio.google.com/apikey](https://aistudio.google.com/apikey)
3. Open `index.html` in your browser
4. Paste your API key when prompted

## Files

```
├── index.html    # Main application
├── kuro.vrm      # 3D model (place your VRM here)
└── README.md
```

## Hosting on GitHub Pages

1. Go to repository **Settings**
2. Click **Pages** in sidebar
3. Set source to `main` branch
4. Your site will be at `https://username.github.io/kuro-ai`

## Customization

**Change personality:** Edit `SYSTEM_PROMPT` in index.html

**Change model:** Replace `kuro.vrm` with your own VRM file

## Credits

- 3D rendering: [Three.js](https://threejs.org)
- VRM support: [@pixiv/three-vrm](https://github.com/pixiv/three-vrm)
- AI: [Google Gemini](https://ai.google.dev)

## License

MIT
