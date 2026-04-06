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

You can also open any command from the **Command Palette** (<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>):

| Command |
|:--------|
| 📸 RecordCode: Take Screenshot |
| 🔴 RecordCode: Start Recording |
| ⏹️ RecordCode: Stop Recording |

---

## 🤖 MCP Tools for AI Agents

The extension provides 4 smart tools that Copilot Chat agents can use autonomously:

| Tool | Description |
|:-----|:------------|
| 📸 **Screenshot** | Take a screenshot and return image data directly to the AI model |
| 🔴 **Start Recording** | Begin screen recording with configurable options |
| ⏹️ **Stop Recording** | Stop recording and extract key frames as images |
| ℹ️ **Recording Status** | Query recording state, duration, and file size |

---

## ⌨️ Keyboard Shortcuts

| Command | Shortcut |
|:--------|:--------:|
| Take Screenshot | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>S</kbd> |
| Start Recording | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>R</kbd> |
| Stop Recording | <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>Alt</kbd> + <kbd>X</kbd> |

---

## 🎯 Recording Triggers

<table>
<tr>
<td>🖥️</td>
<td><strong>Process Trigger</strong></td>
<td>Start recording when a specific process appears — auto-stop when it exits</td>
</tr>
<tr>
<td>⏳</td>
<td><strong>Delay Trigger</strong></td>
<td>Start recording after a configurable countdown</td>
</tr>
<tr>
<td>📐</td>
<td><strong>Stability Auto-Stop</strong></td>
<td>Automatically stop recording when screen becomes visually stable</td>
</tr>
<tr>
<td>🐛</td>
<td><strong>Debug Trigger</strong></td>
<td>Auto-record during debug sessions</td>
</tr>
<tr>
<td>📋</td>
<td><strong>Task Trigger</strong></td>
<td>Auto-record during task execution</td>
</tr>
<tr>
<td>🧪</td>
<td><strong>Test Trigger</strong></td>
<td>Auto-record during test runs</td>
</tr>
</table>

---

## ⚙️ Settings

Customize RecordCode through the settings menu or VS Code settings:

| Setting | Default | Options |
|:--------|:-------:|:--------|
| Output Format | MP4 | MP4 · WebM · GIF |
| Frame Rate | 15 fps | 1 – 60 fps |
| Quality | Medium | Low · Medium · High |
| Output Folder | Workspace `.recordings/` | Custom output path |
| Max Key Frames for AI | 5 | 1 – 20 frames |
| Auto-Stop on Stability | Off | On / Off |
| Stability Threshold | 0.5 | 0 – 100 |
| Stability Checks | 3 | Consecutive stable checks needed |
| Auto-Record on Debug | Off | On / Off |
| Auto-Record on Tasks | Off | On / Off |
| Auto-Record on Tests | Off | On / Off |
| Task Filter | All tasks | Custom glob pattern |

💡 **Tip:** Access recording controls quickly by hovering over the status bar icon.

---

## 📋 Requirements

| Requirement | Details |
|:------------|:--------|
| 🟦 **VS Code** | Version **1.96.0** or higher |
| 🪟 **Platform** | Windows (uses native screen capture) |
| 🎞️ **FFmpeg** | Bundled automatically — no manual setup needed |

---

<div align="center">

Made with 💙 by engineers

</div>

---
