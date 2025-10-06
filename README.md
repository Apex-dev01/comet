# 🌌 Comet - Web Proxy & Games Hub

A feature-rich web proxy and games hub with a stunning space-themed UI. Built with Next.js 14, featuring Ultraviolet proxy technology, multiple game integrations, and advanced privacy features.

## ✨ Features

### 🔒 Proxy Features
- **Ultraviolet Proxy**: High-performance web proxy for unrestricted browsing
- **Bare-Mux Integration**: Advanced request handling
- **About:blank Cloaking**: Hide your browsing activity
- **Custom Rewriter**: URL manipulation and content injection

### 🎮 Games Integration
- **GameDistribution API**: Access to thousands of HTML5 games
- **Ruffle Emulator**: Play Flash games through WebAssembly
- **Unity WebGL Support**: Run Unity games in browser
- **Proxied Game Loading**: All games routed through proxy for access

### 🎨 UI Features
- **Space-Themed Design**: Beautiful blue-hued cosmic interface
- **Tabbed Navigation**: Chrome-like tab management
- **Eruda Dev Tools**: Built-in browser developer tools
- **Responsive Layout**: Works on all devices

## 🚀 Quick Start

### Prerequisites
- Node.js >= 18.0.0
- npm or yarn

### Installation

```bash
# Clone the repository
git clone https://github.com/Apex-dev01/comet.git
cd comet

# Install dependencies
npm install

# Run development server
npm run dev
```

Visit `http://localhost:3000` to see the app.

## 📁 Project Structure

```
comet/
├── app/                    # Next.js 14 App Router
│   ├── layout.tsx         # Root layout with space theme
│   ├── page.tsx           # Home page
│   ├── proxy/             # Proxy routes
│   ├── games/             # Games pages
│   └── cloak/             # About:blank cloaking
├── components/            # React components
│   ├── TabManager.tsx     # Tab management UI
│   ├── ProxyFrame.tsx     # Proxy iframe component
│   ├── GameEmbed.tsx      # Game embedding
│   └── ErudaButton.tsx    # Dev tools button
├── lib/                   # Utilities
│   ├── proxy.ts          # Proxy initialization
│   └── games.ts          # Game loader utilities
├── public/               # Static assets
│   ├── uv/              # Ultraviolet files
│   └── games/           # Game assets
├── middleware.ts         # Next.js middleware for routing
├── next.config.js        # Next.js configuration
├── vercel.json           # Vercel deployment config
└── package.json          # Dependencies
```

## 🔧 Configuration

### Vercel Deployment

1. Push your code to GitHub
2. Import project in Vercel
3. Deploy automatically

The `vercel.json` file is pre-configured for optimal deployment.

### Environment Variables (Optional)

```env
NEXT_PUBLIC_GAME_API_KEY=your_gamedistribution_key
```

## 🎮 Adding Games

### GameDistribution
Games are loaded from GameDistribution's embed API. Add game IDs in `lib/games.ts`.

### Flash Games (Ruffle)
Place SWF files in `public/games/flash/` and they'll be automatically loaded with Ruffle.

### Unity WebGL
Export Unity games to WebGL and place in `public/games/unity/`.

## 🛠️ Development

```bash
# Development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Lint code
npm run lint
```

## 📦 Key Dependencies

- **Next.js 14**: React framework with App Router
- **@titaniumnetwork-dev/ultraviolet**: Web proxy
- **@mercuryworkshop/bare-mux**: Request multiplexing
- **eruda**: Mobile-friendly dev tools
- **React 18**: UI library

## 🎨 Customization

### Theme Colors
Edit the space theme in `app/globals.css`:

```css
:root {
  --space-bg: #0a0e27;
  --space-accent: #4a90e2;
  --space-glow: #6eb5ff;
}
```

### Proxy Settings
Configure proxy behavior in `lib/proxy.ts`.

## 🔐 Privacy & Security

- All traffic routed through Ultraviolet proxy
- About:blank cloaking hides from browser history
- No logging or tracking
- Open source and auditable

## 📝 Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run vercel-build` - Vercel build command
- `npm run lint` - Run ESLint

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

MIT License - see LICENSE file for details

## 🙏 Credits

- Ultraviolet by TitaniumNetwork
- Bare-Mux by MercuryWorkshop
- Game integrations from GameDistribution
- Ruffle Flash emulator

## 🐛 Issues

Found a bug? Please open an issue on GitHub.

## 🌟 Support

If you like this project, please give it a star ⭐

---

Built with ❤️ using Next.js and Ultraviolet
