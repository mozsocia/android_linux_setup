https://www.youtube.com/watch?v=5cVOnXchj2g&ab_channel=Abstractprogrammer


To create a desktop shortcut for Android Studio on Ubuntu, follow these steps:

1. Open a terminal window.

2. Navigate to the `bin` directory inside the Android Studio installation directory. The default installation path is usually `~/Android/android-studio/bin`.

```
cd ~/Android/android-studio/bin
```

3. Create a new desktop entry file using a text editor. For example, with nano:

```
nano ~/Desktop/android-studio.desktop
```

4. In the text editor, paste the following contents, replacing `/path/to/android-studio` with the actual path to your Android Studio installation directory:

```
[Desktop Entry]
Version=1.0
Type=Application
Name=Android Studio
Generick Name=Android IDE
Icon=/path/to/android-studio/bin/studio.png
Exec="/path/to/android-studio/bin/studio.sh" %f
Comment=The Official IDE for Android
Categories=Development;IDE;
Terminal=false
StartupWMClass=android-studio
```

5. Save the file and exit the text editor.

6. To apply the proper permissions to the desktop entry file, run:

```
chmod +x ~/Desktop/android-studio.desktop
```

7. You should now see an Android Studio icon on your desktop. Double-click the icon to launch Android Studio.

Alternatively, you can also create a desktop shortcut using the graphical user interface:

1. Right-click on your desktop and select "Create New > Link to Application".
2. In the "Type a name" field, enter "Android Studio".
3. Click the "Browse..." button next to the "Command" field.
4. Navigate to the `bin` directory inside the Android Studio installation directory (e.g., `~/Android/android-studio/bin`).
5. Select the `studio.sh` file and click "Open".
6. Click "Create".

You should now see an Android Studio icon on your desktop. Double-clicking the icon will launch Android Studio.

Note: If you encounter any issues or if the icon doesn't display correctly, you may need to adjust the `Icon` path in the desktop entry file to match the actual location of the `studio.png` file within your Android Studio installation directory.
