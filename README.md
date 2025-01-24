# ZwiftVoice

A macOS menu bar application that lets you control Zwift using voice commands. Say commands like "boost" or "wave" instead of pressing keys while riding!

## Features

- Voice-activated controls for Zwift
- Lives in your menu bar
- Shows available commands in the menu
- Visual feedback when commands are recognized
- Can be easily toggled on/off

## Available Commands

### Camera Angles (Number Keys)
- "default view" - Default view (1)
- "side view" - Side front-left of the rider (4)
- "rear view" - Rear view (5)
- "bird view" - Bird's eye view (9)

### Rider Actions
- "wave" - Wave hand (F2)
- "ride on" - Give Ride On (F3)
- "photo" - Screen capture (F10)

### HUD Controls
- "watts" - Toggle Watt display (G)
- "hide hud" - Hide HUD elements (H)
- "menu" - Show actions/options menu (Up Arrow)

### Movement Controls
- "u turn" - Perform a u-turn (Down Arrow)
- "left" - Turn left (Left Arrow)
- "right" - Turn right (Right Arrow)
- "boost" - Use power-up (Space)

## Installation

1. Download ZwiftVoice.app
2. Move it to your Applications folder
3. Launch the app
4. Grant required permissions when prompted:
   - Click "Open" if you see a security prompt about running an app from an unidentified developer
   - When prompted for Accessibility permissions:
     1. Open System Settings > Privacy & Security > Accessibility
     2. Click the "+" button
     3. Navigate to Applications
     4. Select ZwiftVoice.app
     5. Toggle the switch ON next to ZwiftVoice

## Usage

1. Make sure ZwiftVoice is running (look for the 🎤 icon in your menu bar)
2. Start Zwift
3. While riding, simply say any of the available commands
4. The menu bar icon will flash ⚡️ when a command is recognized
5. Toggle voice recognition on/off by clicking the menu bar icon and selecting "Active"

## Development Setup

If you want to build the app yourself:

1. Open Xcode
2. Create a new macOS App project:
   - Choose "App" under macOS
   - Set Interface to "SwiftUI"
   - Name it "ZwiftVoice"
   
3. Replace/create these files:
   - `App.swift` - Main app entry point
   - `AppDelegate.swift` - App lifecycle and menu bar handling
   - `VoiceController.swift` - Voice recognition and keystroke simulation

4. In the project settings:
   - Under "Signing & Capabilities", ensure "App Sandbox" is enabled
   - Under "Info", add "Application is agent (UIElement)" and set it to YES
   - Under "Frameworks", add:
     - Cocoa.framework
     - Speech.framework

5. Build and run!

## Requirements

- macOS 11.0 or later
- Microphone access
- Accessibility permissions

## Troubleshooting

1. **App doesn't appear**: Look for the microphone icon (🎤) in your menu bar
2. **Commands not working**: 
   - Check if Accessibility permission is granted
   - Make sure the "Active" menu item is checked
   - Ensure your microphone is working
3. **Zwift not responding**: Make sure Zwift window is active/focused

## Support

This is an open-source project. For issues or feature requests, please submit them on GitHub.

## License

MIT License - Feel free to modify and distribute this app as needed.
