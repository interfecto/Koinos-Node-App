# Release Files

This directory is prepared for future pre-built release files for the Koinos Desktop Node application.

## Current Status

**Pre-built binaries are not currently available.** Users need to compile the application themselves.

Please use the development installation method from the main README to build and run the application.

### Future Releases

Pre-built binaries will be available for:
- **macOS ARM64**: For Apple Silicon Macs (M1, M2, M3, etc.)
- **macOS Intel**: For Intel-based Macs
- **Windows x64**: For Windows 10/11
- **Linux x64**: For Ubuntu/Debian-based systems

## Compilation Instructions

Since pre-built binaries are not available, please compile the application yourself:

```bash
# Clone the repository
git clone https://github.com/interfecto/Koinos-Node-App.git
cd Koinos-Node-App

# Install dependencies
npm install

# Build the application
npm run tauri build

# The built application will be in src-tauri/target/release/bundle/
```

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
