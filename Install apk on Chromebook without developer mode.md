https://www.slashgear.com/886590/how-to-install-apks-on-your-chromebook/

Navigate to Settings > Developers > Linux development environment (Beta) and toggle the Turn On button.
- Click Install on the next window and follow the on-screen prompts.
- Wait for the installation to finish. You'll get a terminal app in your launcher and a new Linux (Beta) section in the Settings menu.
- Now we'll enable ADB debugging. Go to Settings > Linux Beta > Develop Android apps > Enable ADB debugging. Your Chromebook will prompt you to Restart and then click Continue.

Read More: https://www.slashgear.com/886590/how-to-install-apks-on-your-chromebook/

- To move the APK file to the Linux directory, drag and drop it into My Files > Linux files. You might want to rename the APK to make it easier to type into the terminal.
- Now launch the Linux Terminal that we installed in the previous **section.**
- We'll use the Linux APT package manager to install the ADB command-line tool. Enter the following without quotes: "sudo apt install adb". Press Y and hit Enter when prompted.
- The APT package manager will install the necessary packages and drop you back into the terminal when it's done.
- Next, we'll connect ADB to the Chromebook using "adb connect arc." You'll be prompted to allow USB debugging. Hit OK. Keep "Always allow from this computer" checked if you want to interface with your device in the future.
- The terminal should indicate a successful connection.
- With ADB ready, we can finally install Android apps. To install your APK, enter "adb install nameofyourfile.apk" in the terminal. You can either copy-paste the APK file name or type it manually.
- ADB returns "Success" when the installation is complete. You'll find the app shortcut in the Chrome OS launcher.

Read More: https://www.slashgear.com/886590/how-to-install-apks-on-your-chromebook/ 

The special instructions for intel process are important: viz. "adb -s emulator-5554 install"  https://www.slashgear.com/886590/how-to-install-apks-on-your-chromebook/
