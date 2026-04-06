<div align="center">

# 🎬 Record code in 1 click

### Screen capture and video recording for AI agents — directly from VS Code

[![VS Code](https://img.shields.io/badge/VS%20Code-v1.96+-007ACC?logo=visual-studio-code&logoColor=white)](https://code.visualstudio.com/)
[![Version](https://img.shields.io/badge/version-0.1.0-blue)](https://marketplace.visualstudio.com/)

One click. Smart recordings. Zero config needed. Local and private.

</div>

---

## ✨ Features

| Feature | Description |
|:--------|:------------|
| 🎬 **Record in 1 Click** | Start and stop screen recordings from the status bar |
| 📸 **Instant Screenshots** | Capture full screen, specific windows, or custom regions |
| 🤖 **AI-Powered Tools** | 4 MCP tools that Copilot Chat agents can invoke autonomously |
| 🧠 **Smart Key Frames** | Automatically extracts representative frames for AI analysis |
| 😶‍🌫️ **Full local, full private** | All processing is done locally, ensuring your screen never leaves your machine |
| ⏱️ **Process Triggers** | Auto-record when a specific process starts, stop when it exits |
| 🎯 **Event Triggers** | Auto-record on debug sessions, tasks, or test runs |
| 📐 **Stability Detection** | Auto-stop recording when screen becomes visually stable |
| 🎞️ **Multiple Formats** | Export as MP4, WebM, or GIF |
| ⚡ **Bundled FFmpeg** | No manual setup — FFmpeg is included automatically |

---

## 🚀 Quick Start

<table>
<tr>
<td width="60">

**1.**

</td>
<td>

Look for the **RecordCode** button in the **status bar** (bottom-right corner)

</td>
</tr>
<tr>
<td>

**2.**

</td>
<td>

**Hover** over it to see all available actions, or **click** it to toggle recording instantly

</td>
</tr>
<tr>
<td>

**3.**

</td>
<td>

Recordings are saved automatically to your workspace `.recordings/` folder

</td>
</tr>
</table>

You can also open any command from the **Command Palette** (`Ctrl+Shift+P`):

```
RecordCode: Take Screenshot
RecordCode: Start Recording
RecordCode: Stop Recording
```

---

## 🤖 MCP Tools for AI Agents

The extension registers 4 language model tools that Copilot Chat agents can autonomously invoke:

| Tool | Description |
|:-----|:------------|
| 📸 **`recordcode_screenshot`** | Take a screenshot, returns image data directly to model |
| 🔴 **`recordcode_record_start`** | Start screen recording with configurable options |
| ⏹️ **`recordcode_record_stop`** | Stop recording, extract key frames as images |
| ℹ️ **`recordcode_record_status`** | Query recording state, duration, and file size |

---

## ⌨️ Keyboard Shortcuts

| Command | Keybinding |
|:--------|:----------:|
| Take Screenshot | `Ctrl+Shift+Alt+S` |
| Start Recording | `Ctrl+Shift+Alt+R` |
| Stop Recording | `Ctrl+Shift+Alt+X` |

---

## 🎯 Recording Triggers

### Process Trigger

Start recording when a specific process appears, auto-stop when it exits:

```json
trigger: { type: "process", processName: "notepad.exe" }
```

### Delay Trigger

Start recording after a countdown:

```json
trigger: { type: "delay", delay: 5 }
```

### Stability Auto-Stop

Automatically stop recording when screen becomes visually stable:

```json
autoStopOnStability: true
```

### VS Code Event Triggers

Auto-record on debug sessions, tasks, or test runs via settings:

```
recordcode.triggerOnDebug — Auto-record during debug sessions
recordcode.triggerOnTask  — Auto-record during task execution
recordcode.triggerOnTest  — Auto-record during test runs
```

---

## ⚙️ Settings

Customize RecordCode through VS Code settings:

| Setting | Default | Options |
|:--------|:-------:|:--------|
| `recordcode.defaultFormat` | `"mp4"` | `"mp4"` · `"webm"` · `"gif"` |
| `recordcode.defaultFps` | `15` | Frame rate `1`–`60` |
| `recordcode.defaultQuality` | `"medium"` | `"low"` · `"medium"` · `"high"` |
| `recordcode.outputDirectory` | workspace `.recordings/` | Custom output path |
| `recordcode.maxFramesInContext` | `5` | Max key frames returned to AI (`1`–`20`) |
| `recordcode.autoStopOnStability` | `false` | Auto-stop on visual stability |
| `recordcode.stabilityThreshold` | `0.5` | MSE threshold for stability (`0`–`100`) |
| `recordcode.stabilityChecks` | `3` | Consecutive stable checks needed |
| `recordcode.triggerOnDebug` | `false` | Auto-record on debug sessions |
| `recordcode.triggerOnTask` | `false` | Auto-record on task execution |
| `recordcode.triggerOnTest` | `false` | Auto-record on test runs |
| `recordcode.triggerTaskFilter` | `"*"` | Glob pattern to filter tasks |

💡 **Tip:** Access recording controls quickly by hovering over the status bar icon.

---

## 📋 Requirements

- VS Code **1.96.0+**
- **Windows** (uses GDIgrab for screen capture)
- FFmpeg is **bundled automatically** via `@ffmpeg-installer/ffmpeg`

---

<div align="center">

Made with 💙 by engineers

</div>

---
