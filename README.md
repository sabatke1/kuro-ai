Kuro AI

An adorable AI assistant with an anime personality, powered by Groq and featuring real-time voice interaction with lip-sync animation.

Features

3D VRM Avatar - Fully animated anime character with realistic movements
Voice Interaction - Speak to Kuro using your microphone
Real-time Lip Sync - Mouth movements synchronized with audio using Web Audio API
Facial Expressions - Dynamic expressions (happy, surprised, sad, relaxed, blink)
AI Powered - Intelligent conversations using Groq's Llama 3.3 70B model
Mouse Tracking - Kuro follows your cursor with her eyes
Context Awareness - Maintains conversation history for coherent interactions
Ultra Fast - Lightning-fast responses powered by Groq


Quick Start
Option 1: Use Online (Easiest)
Just visit: https://sabatke1.github.io/kuro-ai/
No setup required! Start chatting immediately.
Option 2: Run Locally

Clone the repository:

bash   git clone https://github.com/sabatke1/kuro-ai.git
   cd kuro-ai

Serve locally: (required for CORS)

bash   # Using Python
   python -m http.server 8000
   
   # OR using Node.js
   npx serve
   
   # OR using PHP
   php -S localhost:8000

Open in browser:

   http://localhost:8000

Start chatting! 🎉




🎮 How to Use
Text Chat

Type your message in the input box at the bottom
Press Enter or click the Send button
Kuro will respond with text and voice!

Voice Chat

Click the microphone button
Speak your message
Kuro will transcribe and respond automatically

Interactions

Move your mouse - Kuro's eyes follow your cursor
Watch her expressions - She reacts to different situations
Enjoy the lip sync - Her mouth moves naturally with her voice


🛠️ Technology Stack
TechnologyPurposeThree.js3D rendering engineVRM3D avatar format (VRM 1.0 compatible)Groq APIUltra-fast AI inference (Llama 3.3 70B)ElevenLabsHigh-quality text-to-speechWeb Audio APIReal-time audio analysis for lip syncWeb Speech APIVoice recognition

📁 Project Structure
kuro-ai/
├── index.html          # Main application file
├── kuro.vrm           # 3D VRM avatar model
└── README.md          # This file

⚙️ Configuration
Change AI Personality
Edit the SYSTEM_PROMPT in index.html:
javascriptconst SYSTEM_PROMPT = `You are Kuro, an adorable AI assistant...

Traits:
- Sweet and caring
- Use expressions like "ehehe~", "nyaa~"
- Call user "master" affectionately

Customize this to change Kuro's personality!`;
Change Voice
Edit the VOICE_ID in index.html:
javascriptconst VOICE_ID = 'piI8Kku0DcvcL6TTSeQt'; // Change to any ElevenLabs voice ID
Browse voices at: ElevenLabs Voice Library
Use Your Own VRM Avatar
Replace kuro.vrm with your own VRM file and update:
javascriptconst VRM_URL = 'your-avatar.vrm';
Get VRM avatars at:

VRoid Hub
Booth.pm
Create your own with VRoid Studio


🔑 API Keys
This project uses two APIs:
Groq (AI Chat)

Current: Public key included (limited rate)
Recommended: Get your own free key at console.groq.com
Limit: 14,400 requests/day (free tier)

ElevenLabs (Voice)

Current: Public key included (limited usage)
Recommended: Get your own key at elevenlabs.io
Limit: 10,000 characters/month (free tier)

To use your own keys, update these lines in index.html:
javascriptconst API_KEY = 'your_groq_api_key_here';
const ELEVENLABS_KEY = 'your_elevenlabs_key_here';

🎨 Customization
Adjust Animation Speed
javascript// In the animate() function
leftUpperArm.rotation.z = 1.1 + Math.sin(t * 0.8) * 0.05; // Change 0.8 to adjust speed
Change Background Color
cssbody {
    background: #0a0a0f; /* Change this hex color */
}
Modify Lip Sync Sensitivity
javascript// In the speak() function
vrm.expressionManager.setValue('aa', normalized * 0.8); // Adjust 0.8 (0.0 - 1.0)

🐛 Troubleshooting
Kuro doesn't load

Check console (F12) for errors
Ensure kuro.vrm is in the same folder as index.html
Try using a local server instead of opening the file directly

Voice doesn't work

Check your browser supports Web Audio API (Chrome, Edge recommended)
Ensure your internet connection is stable
Check if ElevenLabs API key is valid

Microphone doesn't work

Grant microphone permissions when prompted
Only works on HTTPS or localhost
Check browser compatibility (Chrome, Edge work best)

AI responses are slow/failing

Check Groq API key is valid
Verify your internet connection
Check rate limits haven't been exceeded


📝 Browser Compatibility
BrowserSupportedNotesChrome✅Best performanceEdge✅Full supportFirefox⚠️Some features limitedSafari⚠️Limited Web Audio supportMobile⚠️Works but performance may vary

🤝 Contributing
Contributions are welcome! Here's how you can help:

Fork the repository
Create a feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request

Ideas for Contributions

 Add more VRM avatar options
 Implement emotion detection
 Add multi-language support
 Create mobile-optimized UI
 Add conversation memory/persistence
 Implement gesture controls
 Add background environment options


📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

🙏 Acknowledgments

Three.js - 3D graphics library
VRM Consortium - VRM format specification
Groq - Ultra-fast AI inference
ElevenLabs - High-quality TTS
Pixiv - three-vrm library


📧 Contact
Project Maintainer: @sabatke1
Issues: GitHub Issues

⭐ Show Your Support
If you like this project, please consider:

Giving it a ⭐ on GitHub
Sharing it with others
Contributing to its development


<div align="center">
Made with ❤️ by the Kuro AI Team
Report Bug · Request Feature
</div>
