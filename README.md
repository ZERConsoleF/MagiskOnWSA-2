## Magisk on WSA

### Usage
1. Fork this repo
1. Go to Action tab and select workflow `Magisk`, click the run button and enter the needed infomation (architecture and magisk apk download link)
1. Wait the action complete and download the artifact
1. Uninstall WSA
1. Unzip the artifact 
1. Enable deveop mode on Windows
1. Open powershell with admin permission and run `Add-AppxPackage -Register .\AppxManifest.xml` under the unzipped artifact directory
1. Launch WSA and enable develop mode, launch the file manager, and wait until the file manager popup
1. `adb connect localhost:58526` to connect` to connect to WSA and install Magisk canary app (23010) (the attached magisk.apk) and launch it
1. Fix the environment as Magisk app will prompt and reboot
1. Enjoy by installing Riru and LSPosed