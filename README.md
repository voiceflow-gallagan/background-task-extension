# Voiceflow Background Task Extension Demo

This repository contains a demo showcasing two custom extensions for Voiceflow: CommandRequest and NotificationExtension. These extensions demonstrate how to implement background tasks and custom notifications in Voiceflow chat widgets.

## Demo Video

Watch the demo in action: [Loom Video](https://www.loom.com/share/cde54b5fdd40408087c4e251a2781d93?sid=df376467-91c1-43e0-ac8b-973bc8a09f71)

## Extensions Overview

### 1. CommandRequest Extension
This extension demonstrates how to trigger custom commands in the Voiceflow Assistant after completing a background task.

**Features:**
- Simulates a background task with configurable delay
- Makes HTTP requests to httpstat.us
- Triggers a custom command in Voiceflow Assistant after completion
- Error handling and logging

**Note:** To use this extension with Commands, you need to request access to the Commands feature from Voiceflow.

### 2. NotificationExtension
This extension shows how to create custom notifications within the Voiceflow chat widget.

**Features:**
- Displays custom notifications with configurable messages
- Smooth fade in/out animations
- Configurable display duration
- Styled notifications with custom CSS
- Error handling and logging

## Voiceflow Project

The Voiceflow project file is included in this repository:
- `Background Task Demo Mar 20 2025.vf`

## Local Development

To run this demo locally:

1. Clone this repository
2. Install dependencies (if any)
3. Run the local server using:
   ```bash
   npx serve
   ```
4. Open your browser and navigate to the provided local URL (typically http://localhost:3000)

## Usage

### CommandRequest Extension
```javascript
{
  type: 'ext_customRequest',
  payload: {
    delay: 5 // Delay in seconds (optional, defaults to 5)
  }
}
```

### NotificationExtension
```javascript
{
  type: 'ext_notification',
  payload: {
    message: 'Your custom message here',
    delay: 5, // HTTP request delay in seconds (optional, defaults to 5)
    anim_delay: 5 // Notification display duration in seconds (optional, defaults to 5)
  }
}
```

## Requirements

- Voiceflow account with access to custom extensions
- Commands feature access (for CommandRequest extension)
- Modern web browser with JavaScript enabled

## License

This project is licensed under the MIT License - see the LICENSE file for details.
