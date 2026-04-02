# LocalFront

LocalFront is a locally-hosted, offline-ready variant of OpenFront—a real-time strategy game focused on territorial control and alliance building. Play without ads and enjoy a fully personalized gaming experience on your own machine.

## 🎮 What is LocalFront?

LocalFront is a complete local implementation of the OpenFront strategy game. Players compete to expand their territory, build structures, and form strategic alliances across various maps based on real-world geography. Unlike the online version, LocalFront runs entirely on your local machine without internet requirements or advertisements.

**Key Differences from OpenFront:**
- ✅ **No Ads** - Play ad-free without interruptions
- ✅ **Completely Local** - No internet connection required after initial setup
- ✅ **Personalized Colors** - Customized UI theme for enhanced visual appeal
- ✅ **Self-Hosted** - Full control over your gaming environment

## 🌟 Core Features

- **Real-time Strategy Gameplay** - Expand your territory and engage in strategic battles
- **Alliance System** - Form alliances with other players for mutual defense and cooperation
- **Multiple Maps** - Play across various geographical regions including Europe, Asia, Africa, and more
- **Resource Management** - Balance your expansion with defensive capabilities
- **Cross-platform** - Play in any modern web browser on Windows, macOS, or Linux

## 📋 Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [npm](https://www.npmjs.com/) (v10.9.2 or higher)
- A modern web browser (Chrome, Firefox, Edge, Safari, etc.)
- 2GB minimum free disk space

## 🚀 Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/LocalFront.git
cd LocalFront
```

### 2. Install Dependencies
```bash
npm ci --ignore-scripts
```

### 3. Start the Development Server
```bash
npm run dev
```

The game will be available at `http://localhost:5173`

### 4. Play Locally
Open your browser and start playing! The game runs entirely on your local machine.

## 🏗️ Development

### Available Commands

```bash
# Development with auto-reload
npm run dev

# Build for production
npm run build-prod

# Build for development
npm run build-dev

# Run tests
npm test

# Run with coverage
npm run test:coverage

# Format code
npm run format

# Lint code
npm lint

# Fix linting issues
npm run lint:fix
```

### Project Structure

```
LocalFront/
├── src/
│   ├── client/       # Client-side game UI and logic
│   ├── server/       # Server-side game logic
│   └── core/         # Shared game mechanics
├── resources/        # Game assets (maps, sprites, sounds, translations)
├── tests/            # Test suites
├── docs/             # Documentation
└── map-generator/    # Tool for generating game maps
```

## 🎨 Customization

LocalFront comes with personalized colors and styling. To further customize:

1. **Colors** - Modify button and UI colors in `src/client/GameModeSelector.ts`
2. **Assets** - Replace game images and sprites in `resources/`
3. **Translations** - Update game text in `resources/lang/`
4. **Maps** - Use the map generator tool to create custom maps

### Removing Ads
Ad-related code and references have been removed throughout the codebase. The game runs completely ad-free.

## 📦 Build & Deployment

### Local Production Build
```bash
npm run build-prod
npm run start:server
```

Your game will be available at `http://localhost:3000`

### Docker Deployment
```bash
docker build -t localfront .
docker run -p 3000:3000 localfront
```

## 🧪 Testing

Run the complete test suite:
```bash
npm test
```

Run tests with coverage:
```bash
npm run test:coverage
```

## 📝 License

LocalFront is based on OpenFront, which is licensed under the **GNU Affero General Public License v3.0**.

Modified versions must preserve copyright notices in reasonably visible locations:
- Footer: "© OpenFront and Contributors"
- Loading screen: "© OpenFront and Contributors"

See the [LICENSE](LICENSE) for complete requirements.

## 🤝 Contributing

Contributions are welcome! Please:

1. Follow the existing code style and conventions
2. Run `npm run format` and `npm run lint:fix` before committing
3. Write tests for new features
4. Update documentation as needed

## 📚 Documentation

- [Architecture](docs/Architecture.md) - System design and components
- [API Documentation](docs/API.md) - Server API reference
- [Authentication](docs/Auth.md) - Authentication system details

## 🐛 Troubleshooting

### Port Already in Use
If port 5173 (dev) or 3000 (production) is already in use, you can specify a different port:
```bash
npm run dev -- --port 5174
```

### Node Modules Issues
Clear node modules and reinstall:
```bash
rm -r node_modules package-lock.json
npm ci
```

### Build Failures
Ensure you're using Node.js v18 or higher:
```bash
node --version
```

## 🎯 Roadmap

- [ ] Enhanced offline support with service workers
- [ ] Local save/replay system
- [ ] Custom map creation UI
- [ ] Additional language translations
- [ ] Performance optimizations

## 📞 Support

For issues and questions:
- Check existing [documentation](docs/)
- Review the [original OpenFront repository](https://github.com/openfrontio/OpenFrontIO)
- Open an issue in your local fork

## 🙏 Acknowledgments

LocalFront is built upon [OpenFront](https://github.com/openfrontio/OpenFrontIO), which itself is a fork/rewrite of WarFront.io. Thanks to all contributors to these projects.

---

**Enjoy your completely local, ad-free strategy gaming experience with LocalFront!** 🎮
