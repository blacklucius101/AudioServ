# AudioServ PC Server

LAN audio server for multi-user Android client streaming. Pairs with [AudioServ Android Client](https://github.com/blacklucius101/AudioServ_android-client).

## Features
- Serve audio libraries to multiple Android devices
- Real-time playback position sync across device groups
- Progressive streaming with chapter support
- No internet required - pure LAN

## Quick Start
1. Download v1.0 release or build from source
2. Configure audio folders in `config.json`
3. Run: `./audioserv --port 3000 --root /path/to/audio`
4. Connect Android clients to `http://YOUR_PC_IP:3000`

## Architecture
- HTTP/JSON API for browsing and control
- WebSocket for live position updates
- Supports MP3/M4B with metadata scanning
