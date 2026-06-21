# Screen Motion Detector for Telegram

Lightweight PyQt6 & Pillow desktop application that monitors real-time screen activity within an adaptive, resizable transparent overlay. Instantly dispatches motion detection alerts and updates to a specified Telegram channel or group.

## Features

- **Adaptive Transparent Frame:** A resizable and draggable red overlay box that marks the active tracking zone. Resize it effortlessly by dragging its edges.
- **Advanced Motion Detection:** Powered by `Pillow (PIL)`, the app tracks pixel deviations inside the safe zone, filtering out noise and subtle shadows to minimize false positives.
- **Telegram Integration:** Sends real-time notifications (`🟢 Start`, `⚠️ Movement detected...`, `🔴 Stop`) using simple HTTP requests via standard Python libraries.
- **Local Configurations Persistence:** Automatically stores your Bot Token and Chat/Channel ID into a localized `config.json` file for swift deployments on future launches.
- **Anti-Spam Controls:** Includes a mandatory 2-second timeout cooldown sequence right after a trigger event to prevent spam cascades.

## Prerequisites & Installation

Make sure you have Python 3.8+ installed on your computer.

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git)
   cd YOUR_REPOSITORY_NAME
