# dlna-np
# DLNA-NP Media Server

A modern, feature-rich DLNA/UPnP media server built with Rust and Tauri, designed for streaming video content to DLNA-compatible devices like Smart TVs, media players, and streaming devices.

<img width="320"  alt="изображение" src="https://github.com/user-attachments/assets/f452a2da-d4c6-4c2f-9f04-d578a3126e1d" />
<img width="320" alt="изображение" src="https://github.com/user-attachments/assets/976a97ed-2814-4b20-adc5-89c0437c7aaa" /> 

## 🌟 Features

### Media Management
- **Playlist Management**: Create and organize multiple playlists from different folders
- **Automatic File Discovery**: Automatically scans folders for video files
- **Real-time Updates**: File system monitoring with automatic playlist refresh
- **Folder Structure**: Support for nested folders with flat or hierarchical view
- **File Statistics**: Track total files, sizes, and enabled content

### DLNA/UPnP Streaming
- **Device Discovery**: Automatic SSDP discovery of DLNA Media Renderers
- **Multi-Device Playback**: Stream to multiple devices simultaneously
- **Device Persistence**: Remember selected devices across sessions
- **Transport Controls**: Play, pause, stop, seek functionality
- **Volume Control**: Real-time volume and mute control via GENA events
- **Position Tracking**: Live playback position monitoring

### Playlist Features
- **Queue Management**: View and manage playback queue
- **Shuffle Mode**: Randomize playback order
- **Repeat Mode**: Loop through playlist continuously
- **Track Navigation**: Previous/Next track with cyclic navigation
- **Auto-Advance**: Automatic progression to next track

### User Interface
- **Modern Design**: Clean, responsive interface with dark mode support
- **Mobile Optimized**: Touch-friendly controls for mobile devices
- **Real-time Updates**: Live statistics and playback status
- **Drag & Drop**: Easy file management
- **Collapsible Sections**: Organize content efficiently


## 🔧 Configuration

The server runs on port 3000 by default. Configuration is stored in `config.json`:

```json
{
  "port": 3000
}
```

## 📖 Usage

### Adding Playlists

1. Click "Add New Playlist"
2. Enter a name for your playlist
3. Select a folder containing video files
4. Choose between flat or hierarchical view
5. Click "Create"

### Streaming to Devices

1. Click "Select Device" to scan for DLNA devices
2. Select one or more target devices
3. Click on any video file to start playback
4. Use the playback controls to manage playback

### Volume Control

Volume control works via UPnP GENA events:
- Real-time synchronization with device volume
- Adjust volume using the slider (applies on release)
- Mute/unmute with the volume button
- Automatic updates when volume changes on device

### Playlist Playback

1. Click the play button on a playlist to start
2. Use shuffle/repeat buttons to control playback mode
3. View queue to see upcoming tracks
4. Click any track in queue to jump to it

## 🎯 Supported Video Formats

- MP4 (.mp4, .m4v)
- AVI (.avi)
- MKV (.mkv)
- MOV (.mov)
- WMV (.wmv)
- FLV (.flv)
- WebM (.webm)
- MPEG (.mpg, .mpeg)
- Transport Stream (.ts, .mts)

## 🎨 User Interface Features

### Dark Mode
- Automatic theme detection
- Manual toggle available
- Persistent preference storage

### Real-time Updates
- Live playback position
- Automatic volume synchronization
- File system change detection
- Device status monitoring

## 📄 License

MIT License - see LICENSE file for details

## 📞 Support

For issues and questions, please open an issue on the GitHub repository.

---

**Note**: This is a home media server designed for local network use. Always ensure you have the rights to stream the content you're sharing.








