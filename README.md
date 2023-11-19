# OBSKeyTriggeredTextOverlay
A tool that creates a window with text upon a hotkey press. This window will always be on top of everything. Made by Wumpie.

The actual commit history is on my Python Projects Repository
From commit ChristanVersteeg/python_projects@f68f81a to ChristanVersteeg/python_projects@f8c1b28

# Latest Release: https://github.com/ChristanVersteeg/OBSKeyTriggeredTextOverlay/releases

# Setup
1. Download Python 3.11.6. Make sure that it's added to your PATH. Python's 3.11.6 installer (for Windows) is given with this release for ease of access. You will also need to install the keyboard library. You can do this by going to your cmd (once Python is installed) and typing `pip install keyboard` in it.
2. If you do not have OBS yet, download the latest release (30.0.0 as of release) https://obsproject.com/download
3. Open your OBS, then `Tools > Scripts`, within that menu, click `Python Settings`, from there click browse and assigned your installed Python 3.11.6.
![image](https://github.com/ChristanVersteeg/OBSKeyTriggeredTextOverlay/assets/90323125/bc5d2e2f-e691-4aea-b24f-4438eed3eaa2)
4. Download the Python files; `InteractiveLabelManager.py` and `OBSKeyTriggeredTextOverlay.py`. They're both within the `OBSKeyTriggeredTextOverlayScripts.zip` folder brought with this release.
5. Store these in a place where you want them, you'll always need these two to run the program. 
6. Then go back to `Tools > Scripts`, within the menu click `Scripts`, then click the plus icon in the bottom left, and browse to the downloaded OBSKeyTriggeredTextOverlay.py and add it to the list.
7. Once it's added to the list you should get a view like this:
![image](https://github.com/ChristanVersteeg/OBSKeyTriggeredTextOverlay/assets/90323125/8fd37afe-fbfe-4f5e-8364-465a01532a96)
8. If the first field (Python Script Path) has not assigned itself, click the browse button, and assign it the InteractiveLabelManager.py you've downloaded to the field.
9. That's it! Now you should be able to open the text overlay with the key `9`, if you prefer to assign another hotkey, you can do that by just clicking the hotkey dropdown and choosing a key of your liking. You can also move around the text overlay by just holding left mouse button on it and dragging. It will save it's last position that it was in.
10. You can tinker with the rest of the settings to get the text as you need. Don't forget to press the refresh button bottom left of the scripts window when you changed the settings, else the new settings won't be applied to the text overlay.

### Data
Config files are stored within your appdata, in the folder `<Disc>:\Users\<UserName>\AppData\Local\OBSKeyTriggeredTextOverlayConfig`. Note, changing the `.json` file directly will not work, OBS will override it. The settings in OBS are leading. You can change the `window_position.txt` manually if you really wanted to. It will use what you changed it to upon script refresh. Note that if you do not adhere to the formatting of the `window_position.txt` it will break. The json will be fine since OBS overrides it, always. If you delete the config files they will be regenerated again.
