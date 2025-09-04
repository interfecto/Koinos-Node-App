# Koinos Node Desktop App v0.4.0 Release

**Release Date:** September 3, 2025  
**Platform:** macOS (Apple Silicon - aarch64)

## 🎯 Release Contents

This release folder contains the EXACT working version that has been tested and verified.

### Files Included

1. **koinos-node-app_0.4.0_aarch64.dmg** (4.8 MB)
   - Ready-to-install disk image for macOS
   - Drag and drop installation
   - Signed and notarized (if applicable)

2. **koinos-node-app.app**
   - The actual application bundle
   - Can be directly copied to Applications folder

3. **koinos-node-app-v0.4.0-source.tar.gz** (2.1 MB)
   - Complete source code archive
   - Does NOT include build artifacts (node_modules, target/, dist/)
   - Clean git archive for developers

4. **checksums.sha256**
   - SHA-256 checksums for verification
   - Verify downloads are not corrupted

## ✅ Verified Features

This exact build has been tested with the following confirmed working:
- ✅ Docker path detection (including Docker Desktop app path)
- ✅ Node status monitoring in real-time
- ✅ Sync progress tracking
- ✅ Resource usage monitoring (CPU, Memory, Disk)
- ✅ Start/Stop/Restart controls
- ✅ Auto-installation of Docker (guided)
- ✅ Blockchain snapshot download with resume
- ✅ Debug console for troubleshooting

## 📦 Installation Instructions

### For End Users (DMG):
1. Download `koinos-node-app_0.4.0_aarch64.dmg`
2. Double-click to mount the DMG
3. Drag the Koinos Node App to your Applications folder
4. Launch from Applications
5. Follow the setup wizard

### For Developers (Source):
1. Download `koinos-node-app-v0.4.0-source.tar.gz`
2. Extract: `tar -xzf koinos-node-app-v0.4.0-source.tar.gz`
3. Install dependencies:
   ```bash
   cd koinos-node-app-v0.4.0
   npm install
   ```
4. Run development mode:
   ```bash
   npm run tauri dev
   ```
5. Build production:
   ```bash
   npm run tauri build
   ```

## 🔒 Verification

Always verify downloads using the provided checksums:

```bash
shasum -a 256 -c checksums.sha256
```

Expected output:
```
koinos-node-app_0.4.0_aarch64.dmg: OK
koinos-node-app-v0.4.0-source.tar.gz: OK
```

## 📋 System Requirements

- **macOS:** 11.0 or later (Big Sur+)
- **Architecture:** Apple Silicon (M1/M2/M3)
- **Docker:** Docker Desktop (will guide installation if missing)
- **Storage:** ~60GB free space for blockchain data
- **RAM:** 8GB recommended (6GB minimum)

## 🐛 Known Issues & Fixes Applied

### Fixed in This Release:
- Docker path detection now includes `/Applications/Docker.app/Contents/Resources/bin/docker`
- Node status properly updates in the UI
- Sync progress accurately reflects blockchain height

## 🔧 For Contributors

### Key Source Files (Clean, No Build Artifacts):
```
src/
├── components/         # React UI components
├── App.tsx            # Main application logic
src-tauri/
├── src/
│   ├── node_manager.rs    # Docker & node management
│   ├── auto_installer.rs  # System requirements installer
│   ├── logger.rs          # Logging system
│   └── lib.rs            # Tauri command handlers
```

### Build Tools Required:
- Node.js 18+
- Rust 1.70+
- npm or yarn
- Tauri CLI

## ⚠️ IMPORTANT NOTES

1. **This is the EXACT version that was tested and confirmed working**
2. **DO NOT modify the DMG or app bundle** - Use as-is for distribution
3. **Source archive is clean** - No node_modules, no target/, no dist/
4. **For Intel Macs** - A separate build may be needed (x86_64)

## 📞 Support

- GitHub Issues: [Report bugs here]
- Discord: [Community support]
- Documentation: See README.md in source

## 📜 License

MIT License - See LICENSE file in source code

---

**Integrity Notice:** This release folder contains the exact binaries that were tested and verified working. Any modifications may affect functionality.