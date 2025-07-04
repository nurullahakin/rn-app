## Start Android Device.app

Steps:

-   Automator.app
-   Document type: Application
-   Action: Run Shell Script (drag-and-drop)
-   Enter the script
-   Save

The script:

```bash
nohup ~/Library/Android/sdk/emulator/emulator -avd Medium_Phone_API_36.0 > /dev/null 2>&1 &
```

Notes:

- `Medium_Phone_API_36.0` is arbitrary. Choose whatever device you want to use. To list the available devices, run:

```bash
~/Library/Android/sdk/emulator/emulator -list-avds
```
