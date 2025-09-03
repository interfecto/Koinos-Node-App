# Release Files

This directory contains pre-built release files for the Koinos Desktop Node application.

## Current Releases

### v0.4.0 (Beta)

- **macOS ARM64**: `koinos-node-app_0.4.0_aarch64.dmg.zip` (contains DMG)
  - Compatible with Apple Silicon Macs (M1, M2, M3, etc.)
  - Size: ~50MB
  - Requires macOS 10.15+ (Catalina or later)
  - **Note**: DMG is packaged in ZIP to prevent GitHub download corruption

### Planned Releases

- **macOS Intel**: For Intel-based Macs
- **Windows x64**: For Windows 10/11
- **Linux x64**: For Ubuntu/Debian-based systems

## Installation Instructions

### macOS

1. Download the ZIP file for your system
2. Double-click the ZIP file to extract the DMG
3. Double-click the extracted DMG file to mount it
4. Drag the Koinos Node application to your Applications folder
5. Launch the application from Applications or using Spotlight

### Why ZIP instead of DMG?

**Problem**: DMG files often get corrupted when downloaded directly from GitHub.

**Solution**: We package the DMG in a ZIP file to prevent corruption during download. This is a common workaround for GitHub's binary file handling issues.

### System Requirements

- **macOS**: 10.15+ (Catalina or later)
- **Docker Desktop**: Required for node operation
- **RAM**: Minimum 8GB, recommended 16GB+
- **Storage**: At least 60GB free space for blockchain data

## Beta Software Notice

⚠️ **This is BETA software** - Use at your own risk. See the main README for full disclaimer.

## Future Releases

Additional platform releases will be added here as they become available:
- macOS Intel (x86_64)
- Windows (x64)
- Linux (x64)

## Verification

To verify the integrity of release files, checksums will be provided in future releases.
