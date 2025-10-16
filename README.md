# MP3 Player App - React Native

A fully-featured MP3 player application built with React Native for Android devices.

## Features

### Core Features
- ✅ **Audio Playback Control**: Play, pause, stop, next, previous
- ✅ **Audio Library Management**: Browse and display audio files from device storage
- ✅ **Progress Control**: Interactive seek bar with current time and duration display
- ✅ **Volume Control**: Adjustable playback volume with slider
- ✅ **Playlist Management**: Create, edit, and delete custom playlists
- ✅ **Background Playback**: Continue playing music when app is minimized
- ✅ **Audio File Metadata**: Display song title, artist, album information

### Advanced Features
- ✅ **Shuffle Mode**: Randomize track playback order
- ✅ **Repeat Modes**: Off, repeat queue, repeat single track
- ✅ **Search Functionality**: Find songs, artists, and albums quickly
- ✅ **Modern UI Design**: Material Design-inspired dark theme
- ✅ **Mini Player**: Quick access controls from main screen
- ✅ **File Browser**: Automatic detection of music files on device
- ✅ **Responsive Design**: Optimized for various Android screen sizes

## Tech Stack

- **Framework**: React Native 0.72.6
- **Audio Library**: react-native-track-player v4.0.1
- **Navigation**: React Navigation v6
- **File System**: react-native-fs
- **UI Components**: react-native-vector-icons, react-native-slider
- **Styling**: react-native-linear-gradient

## Installation & Setup

### Prerequisites
- Node.js (>= 16.x)
- React Native CLI
- Android Studio
- Android SDK (API level 21+)
- Java Development Kit (JDK 11+)

### Steps

1. **Clone and Install Dependencies**
   ```bash
   cd PROJECT-01
   npm install
   ```

2. **Android Setup**
   ```bash
   npx react-native run-android
   ```

3. **Link Vector Icons (if needed)**
   ```bash
   npx react-native link react-native-vector-icons
   ```

### Permissions Required
- `READ_EXTERNAL_STORAGE`: Access music files on device
- `WRITE_EXTERNAL_STORAGE`: Save playlists and app data
- `WAKE_LOCK`: Keep device awake during playback
- `FOREGROUND_SERVICE`: Background music playback

## Project Structure

```
src/
├── App.js                 # Main application component
├── context/
│   └── MusicContext.js    # Global music state management
├── screens/
│   ├── HomeScreen.js      # Main music library screen
│   ├── PlayerScreen.js    # Full-screen music player
│   └── PlaylistScreen.js  # Playlist management
├── services/
│   └── PlaybackService.js # Background audio service
└── utils/
    └── musicUtils.js      # Music file utilities
```

## Usage Guide

### First Launch
1. Grant storage permissions when prompted
2. The app will automatically scan for music files
3. Tap any song to start playing

### Creating Playlists
1. Navigate to "Playlists" tab
2. Tap "Create New Playlist"
3. Add songs from your library
4. Manage playlist contents as needed

### Player Controls
- **Tap song**: Play/pause current track
- **Swipe**: Navigate between tracks (in full player)
- **Seek bar**: Jump to specific time in track
- **Volume slider**: Adjust playback volume
- **Shuffle/Repeat**: Toggle playback modes

## Supported Audio Formats

- MP3 (.mp3)
- M4A (.m4a)
- AAC (.aac)
- WAV (.wav)
- FLAC (.flac)
- OGG (.ogg)

## Troubleshooting

### Common Issues

1. **No music files found**
   - Ensure music files are in `/Music` or `/Download` folders
   - Check storage permissions are granted
   - Try the "Refresh" button

2. **Audio not playing**
   - Check device volume settings
   - Ensure audio files are not corrupted
   - Restart the app if needed

3. **Background playback not working**
   - Check battery optimization settings
   - Ensure foreground service permission is granted

## Development

### Building for Release
```bash
cd android
./gradlew assembleRelease
```

### Testing
```bash
npm test
```

## Future Enhancements

- [ ] Audio equalizer with preset modes
- [ ] Sleep timer functionality
- [ ] Recently played history
- [ ] Album artwork extraction
- [ ] Crossfade between tracks
- [ ] Audio effects and filters
- [ ] Cloud storage integration
- [ ] Social sharing features

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- React Native Community for excellent libraries
- Material Design for UI inspiration
- Contributors and testers

---

**Author**: Shiva  
**Version**: 1.0.0  
**Platform**: Android  
**Framework**: React Native
