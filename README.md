# Rclone-Google-Drive
Rclone Configuration Steps for Google Drive

### Background
As a newcomer to Linux, I needed a reliable way to mount Google Drive. The default "Online Accounts" integration works fine with the native file manager, but it struggles with third-party applications. When opening files through external apps, the system exposes the Google Drive file IDs instead of their actual names, turning file selection into a guessing game.

### Solution
To bypass this limitation, this project uses [rclone](https://rclone.org). By creating a dedicated project in the Google Cloud Console and generating private OAuth credentials for the Google Drive API, rclone can authenticate directly and mount the folder as a standard local filesystem, ensuring full compatibility and correct file names across the entire OS.

> **Note:** This project was created for my personal use only, but it is shared here to serve as a rough guide in case you are facing the same issue.
