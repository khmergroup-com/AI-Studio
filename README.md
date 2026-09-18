# 📖 AI Studio: Complete User Guide

Welcome to **AI Studio**! AI Studio is a next-generation desktop creative suite designed for content creators, musicians, translators, and video editors. Powered by cutting-edge local and cloud AI models, AI Studio lets you dub videos across languages, clone voices, craft stunning music visualizer videos with synced karaoke lyrics, and export high-definition media with zero external dependencies.

---

## 📑 Table of Contents
1. [System Requirements & Installation](#1-system-requirements--installation)
2. [Interface Overview & Navigation](#2-interface-overview--navigation)
3. [Module 1: AI Video Dubbing Studio](#3-module-1-ai-video-dubbing-studio)
4. [Module 2: AI Music & Lyric Video Studio](#4-module-2-ai-music--lyric-video-studio)
5. [Module 3: Voice Cloning & Voice Design](#5-module-3-voice-cloning--voice-design)
6. [Module 4: Text-to-Speech (TTS) Studio](#6-module-4-text-to-speech-tts-studio)
7. [Project Management & Auto-Save](#7-project-management--auto-save)
8. [Settings & AI Provider Configuration](#8-settings--ai-provider-configuration)
9. [In-App Auto-Updates](#9-in-app-auto-updates)
10. [Troubleshooting & FAQ](#10-troubleshooting--faq)

---

## 1. System Requirements & Installation

### System Requirements
- **Operating System**: macOS 12.0 (Monterey) or later (Optimized for Apple Silicon M1/M2/M3/M4; Intel supported).
- **RAM**: 8 GB minimum (16 GB recommended for local Whisper and MLX neural processing).
- **Storage**: At least 3 GB of free disk space for application files and models.
- **FFmpeg**: **Embedded!** You do **not** need to install FFmpeg via Homebrew; AI Studio includes a self-contained, notarized FFmpeg engine.

### Installing AI Studio
1. Download the latest `AI_Studio_x.x.x_aarch64.dmg` from the [Official Releases](https://github.com/khmergroup-com/AI-Studio/releases).
2. Double-click the downloaded `.dmg` file.
3. Drag **AI Studio** into your **Applications** folder.
4. Launch **AI Studio** from Launchpad or Finder.
5. On first launch, grant the necessary microphone and file storage permissions when prompted.

---

## 2. Interface Overview & Navigation

The top navigation bar provides quick access to all studio suites:
- **Dubbing (`/`)**: Video translation, transcription, multi-speaker dubbing, and subtitle editor.
- **Music Studio (`/music`)**: Music visualizer, lyric synchronization, vinyl turntable, and social video generator.
- **Voice Studio (`/voice`)**: Voice cloning from audio samples and voice design.
- **TTS (`/tts`)**: Text-to-Speech generation and multi-voice script reader.
- **Instructions (`/instructions`)**: Quick in-app reference guide.
- **Settings (`/settings`)**: API keys, local hardware acceleration, and system telemetry.
- **Header Controls**:
  - **Status Badge**: Displays backend engine status (🟢 *Backend Online*).
  - **Logs Toggle**: Live streaming console logs for debugging.
  - **Update Badge**: Automatically notifies you when a new release is available.

---

## 3. Module 1: AI Video Dubbing Studio

The Dubbing Studio automates the full video localization workflow from raw video to a synchronized, multi-speaker dubbed video.

```
[Upload Video] ➔ [AI Speech-to-Text] ➔ [Speaker Diarization] ➔ [Multi-Language Translation] ➔ [Voice Dubbing] ➔ [Export Video]
```

### Step-by-Step Workflow:
1. **Upload Source Video**:
   - Drag and drop your `.mp4` or `.mov` file into the upload zone.
   - Choose your original video audio language (or leave on **Auto-Detect**).
2. **Automatic Speech Recognition (Whisper)**:
   - Select your transcription model:
     - **Local Apple Silicon (MLX Whisper)**: Runs 100% offline at ultra-fast speeds using your Mac's Neural Engine.
     - **OpenAI Whisper API**: High accuracy cloud transcription.
3. **Speaker Diarization**:
   - Automatically detects and tags distinct speakers (Speaker 1, Speaker 2, etc.) using Pyannote Audio.
4. **Translation**:
   - Select target language (English, Khmer, Spanish, French, Chinese, Japanese, etc.).
   - Choose translation provider: **Google Translate (Free)**, **OpenAI GPT-4o**, or **Google Gemini**.
5. **Voice Assignment & Voice Dubbing**:
   - Assign different voices to each speaker.
   - Use built-in neural voices (EdgeTTS) or your own custom cloned voices (VoxCPM2).
   - Adjust speech rate, pitch, and volume.
6. **Multi-Track Subtitle Editing**:
   - Edit timestamps, text, and positioning (`Top`, `Middle`, `Bottom`, or drag directly on stage).
   - Choose Khmer typography (**Moul**, **Battambang**, **Kantumruy Pro**) or Latin fonts.
7. **Export Synced Video**:
   - Click **"Sync with Video"** to render the final video with burned-in subtitles, mixed audio, and original background preservation.

---

## 4. Module 2: AI Music & Lyric Video Studio

The Music Studio transforms songs and voice tracks into viral, visually captivating music videos for YouTube, TikTok, Facebook Reels, and Instagram.

### 1. Canvas Dimensions & Aspect Ratios
Switch aspect ratios instantly with real-time responsive stage scaling:
- **16:9 (1920×1080)**: Standard YouTube & widescreen monitors.
- **9:16 (1080×1920)**: Vertical video for TikTok, YouTube Shorts, and Instagram Reels.
- **1:1 (1080×1080)**: Square format for Instagram posts.
- **4:5 (1080×1350)**: Portrait format for social feeds.

### 2. The 8-Track Multi-Layer Timeline
The Music Studio timeline gives you granular control over every visual and audio element:
- **Track 1 (Song Title)**: Enter track title, pick font size, font family, color, and drag anywhere on stage.
- **Track 2 (Artist Name)**: Enter artist name or credits, style and position freely.
- **Track 3 (Synced Lyrics)**: Import `.lrc`, `.srt`, `.vtt`, or `.txt` files. Lyrics highlight synchronously with vocal timing.
- **Track 4 (Audio Visualizer)**: Select reactive visualizer style and sensitivity.
- **Track 5 (Ambient Particles)**: Overlay dynamic floating particles.
- **Track 6 (Center Avatar / Vinyl Disc)**: Upload cover art or artist avatar.
- **Track 7 (Main Audio Track)**: Instrumental or primary song file.
- **Track 8 (Voice / Secondary Track)**: Vocal track or secondary commentary with individual mute/solo controls.

### 3. Visualizer Styles
- **Circular Spectrum**: High-definition audio spectrum bars radiating 360° outward from the center vinyl turntable.
- **Radial Waves**: Concentric pulsating rings expanding with bass frequencies.
- **Bottom Equalizer Bars**: Sleek equalizer spectrum bars flush with the bottom of the video.
- **Sine Waveform**: Oscilloscope wave with glowing audio-reactive amplitude.
- **Color Themes**: **Neon** (Cyan / Magenta / Purple), **Sunset** (Yellow / Orange / Red), **Golden** (Gold / Amber), **Fire** (Crimson / Flame).

### 4. Interactive Stage Drag & Drop
Click and drag any element directly on the live video preview to reposition it:
- Drag the **Song Title** or **Artist Name** to header, bottom, or corners.
- Drag the **Center Avatar** to any focal point on stage. The circular visualizer follows the avatar in real time.
- Drag **Karaoke Subtitles** to your desired reading level.
- Click **"Center"** in the track controls to snap an element back to the exact middle.

### 5. Vinyl Record Animation
- Toggle **Spinning Vinyl** to make your avatar spin smoothly like a real turntable record while playing and in exported videos.
- Includes realistic center spindle hole and glowing perimeter accent ring.

### 6. Exporting High-Definition MP4
1. Click the purple **"Export Video"** button in the header or toolbar.
2. Select your destination file path in the native macOS Save Dialog.
3. The embedded FFmpeg engine encodes the video using Apple Hardware Acceleration (`h264_videotoolbox`):
   - Fast multi-layer rendering at 30/60 FPS.
   - Crystal-clear 320kbps AAC stereo audio.
   - High-bitrate H.264 video ready for immediate social upload.

---

## 5. Module 3: Voice Cloning & Voice Design

The Voice Studio allows you to create custom AI voices from short audio samples.

### Voice Cloning (Instant Voice Clone)
1. Navigate to `/voice`.
2. Click **"New Voice Clone"**.
3. Upload a clean, 10–60 second audio recording of the speaker without background noise or music.
4. Enter the speaker's name and native language.
5. Click **"Train Voice Profile"**.
6. Once processed, the cloned voice becomes immediately available across the Dubbing Studio and TTS Studio!

### Voice Design (Synthetic Persona)
- Create entirely synthetic voices by defining gender, pitch, timbre, accent, and emotional delivery.

---

## 6. Module 4: Text-to-Speech (TTS) Studio

The TTS Studio is designed for narration, audiobooks, podcasts, and video voiceovers.

1. Navigate to `/tts`.
2. Enter or paste your script text into the editor.
3. Select your voice provider (**EdgeTTS** for standard natural voices or **Custom Voice Clone**).
4. Select the target language and voice persona.
5. Adjust speech rate (`-50%` to `+100%`) and volume.
6. Click **"Generate Audio"** to preview in real-time.
7. Download audio as `.wav` or `.mp3`, or import it directly into Dubbing or Music Studio!

---

## 7. Project Management & Auto-Save

AI Studio automatically protects your creative work against unexpected crashes or power outages.

### Auto-Saving Drafts
- Every change made in the Music Studio (lyrics, titles, avatar position, colors, track visibility) is automatically saved in the background.
- Collision prevention ensures your project is saved under unique filenames (e.g., `PROJECT_2026-09-18.pr`, `PROJECT_2026-09-18_1.pr`).

### Project Library
- Click **"Projects"** in the toolbar to open your project library.
- View project creation dates, video aspect ratio, audio durations, and thumbnail previews.
- One-click project restoration restores all tracks, media assets, and canvas coordinates instantly.
- Delete unwanted drafts or export project bundles (`.pr`) to share with collaborators.

---

## 8. Settings & AI Provider Configuration

Navigate to `/settings` to configure your API credentials and preferences:

### Supported Providers
- **OpenAI**: Enter your API key (`sk-...`) for Whisper transcription and GPT-4o translations.
- **Google Gemini**: Enter your Gemini API key for lightning-fast, high-quality translations.
- **Hugging Face**: Enter your User Access Token to download local speaker diarization models.
- **Local Apple Silicon (MLX)**: Enable local GPU/Neural Engine acceleration on M-series Macs for completely offline, private processing.

All API keys are securely stored locally in your encrypted macOS keychain and local app directory (`~/Library/Application Support/AI Studio/`).

---

## 9. In-App Auto-Updates

AI Studio features a built-in auto-update system powered by Tauri v2 and Minisign cryptographic verification.

1. **Automatic Detection**: 4 seconds after launching the app, AI Studio quietly checks the [Official Release Hub](https://github.com/khmergroup-com/AI-Studio) for updates.
2. **Notification Badge**: When a new version is released, a glowing update badge appears in the header and Settings menu.
3. **Interactive Update Dialog**:
   - View release notes and changelog.
   - Click **"Download & Install Update"**.
   - Watch live download progress.
4. **1-Click Relaunch**: Once verified, click **"Restart AI Studio"** to relaunch into the new version with all your projects intact!

---

## 10. Troubleshooting & FAQ

### Q: Why is my exported video taking a few minutes to render?
**A:** Rendering high-definition video with multi-layer audio spectrums, particle physics, and ASS karaoke text requires significant computation. On Apple Silicon Macs (M1/M2/M3/M4), AI Studio leverages `h264_videotoolbox` hardware encoding to maximize speed. For faster exports, shorten the audio length or close intensive background apps.

### Q: Do I need an internet connection to use AI Studio?
**A:** No! Video dubbing with local MLX Whisper, local Edge/offline voice models, and Music Studio video exports can all run 100% offline on your device. An internet connection is only needed when using cloud providers (OpenAI, Gemini) or downloading software updates.

### Q: What audio and video formats are supported?
- **Video Input**: `.mp4`, `.mov`, `.m4v`, `.webm`, `.mkv`
- **Audio Input**: `.mp3`, `.wav`, `.m4a`, `.aac`, `.flac`, `.ogg`
- **Lyrics Input**: `.lrc` (synced karaoke), `.srt`, `.vtt`, `.txt`
- **Image/Avatar Input**: `.png`, `.jpg`, `.jpeg`, `.webp`
- **Video Export**: High-Definition `.mp4` (H.264 / AAC)

### Q: Where are my projects and media stored?
All files, recordings, and databases are stored in your local application directory:
- **macOS**: `~/Library/Application Support/AI Studio/` (or your custom directory set in Settings).

---

## 🤝 Community & Support
- **Release Hub**: [github.com/khmergroup-com/AI-Studio](https://github.com/khmergroup-com/AI-Studio)
- **Report an Issue**: Submit bug reports and feature requests on our GitHub Issues page.
- **License**: AI Studio Commercial EULA (see [LICENSE](file:///Users/sokhapen/Documents/videodubbing/LICENSE)).
