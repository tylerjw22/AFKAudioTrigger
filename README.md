# AFK Audio Trigger

AFK Audio Trigger is a lightweight Windows application that listens to the audio of a selected program and triggers actions when a sound threshold is exceeded. It’s perfect for automating interactions or notifications based on audio cues.

---

## Features

- Listen to audio from a specific application.
- Trigger actions when volume exceeds a defined threshold.
- Configurable cooldown between triggers.
- Logbox to track triggers
- Visual indicator for listening status.
- Supports custom hotkeys and settings.
- Minimalist, dark-themed interface.

---

## Installation

1. **Download the ZIP** from the [releases page](https://github.com/mori227/AFKAudioTrigger/releases/).

2. **Important:** Before extracting/unzipping, unblock the ZIP:
   - Right-click the ZIP → Properties → Check **Unblock** → Apply
   - Then extract it to your preferred location.

3. Run `AFKAudioTrigger.exe` from the extracted folder.

> ⚠ Failure to unblock the ZIP may cause the app to crash immediately on launch.

---

## Usage

1. **Open the app** by running `AFKAudioTrigger.exe`.

2. **Add an application**  
   - Click the **Add** button and select the `.exe` of the program you want to monitor.

3. **Calibrate the audio**  
   - Start calibration from the **Settings** menu.  
   - Play or recreate the sound you want the app to detect so it can automatically set the sensitivity threshold.

4. **Start monitoring**  
   - Press **Start** to begin listening.  

5. **Monitor triggers**  
   - The app will detect the sound and perform the configured action when it exceeds the threshold.  
   - Stop monitoring anytime by pressing **Stop**.

6. Clear log output with **Clear**.

---

## Troubleshooting

- **App crashes on launch**
  - Make sure the ZIP was **unblocked** before extraction.
  - Check that `Resources\images\icon.ico` exists and is not blocked.
  
- **App cannot detect audio**
  - Ensure the target application is running.
  - Make sure you added the correct `.exe`.
  - Adjust the **Volume Sensitivity** in settings.

- **Triggers not firing**
  - Check the cooldown setting; a high cooldown may prevent frequent triggers.
  - Ensure the audio of the target application is above the threshold.

- **UI or indicator issues**
  - Make sure your system supports .NET 9.0 or later.
  - Run as administrator if certain hotkey or input functions fail.

---

## FAQ

**Q: How do I find my exe if its not appearing in the process window?**  
A: Locate the program you want to monitor, right-click its shortcut or executable file, select **Properties**, and look under **Target** or **Location** to find the full path to the `.exe` file, then go to "Add" -> "Browse" and enter that file location in the file explorer.

**Q: What does "recreate a sound" mean when calibrating?**  
A: It means you should play or make the exact sound you want the program to detect while calibration is running. The program will listen and determine the proper threshold level for that sound.

**Q: Why does my app need to be unblocked?**  
A: Windows sometimes flags downloaded ZIP files or executables from the internet. Right-click the file, select **Properties**, and click **Unblock** to allow the program to run correctly.

**Q: What do the settings do?**  
A: You can adjust sensitivity, cooldown times, and the key the program presses when a sound is detected. Calibration will help set the optimal sensitivity automatically.

**Q: Can I monitor multiple applications at once?**  
A: Currently, the program only monitors one application at a time. You can switch between applications using the **Add** button.

**Q: What happens if my application closes while monitoring?**  
A: The program will stop listening and display an alert in the interface. You’ll need to start monitoring again once the application is running.

**Q: Do I need to keep the app open?**  
A: Yes, the app must remain running to detect audio and trigger actions.


---

## License

Made by **tylerjw22**. Use responsibly. 

---

## Support

For help and updates, join the [Discord](https://discord.gg/2jJSVy9Jju) or email: `afkaudiotriggerhelp@gmail.com`
