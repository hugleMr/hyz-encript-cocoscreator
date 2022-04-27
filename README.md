# hyz-encript
This artice : https://forum.cocos.org/t/topic/124553

Cocoscreator is encrypted and confused. Based on 2.4.5, it is theoretically applicable to engine 2.4.0-2.4.6. The most important thing is open source.

![screenshot](https://raw.githubusercontent.com/hugleMr/hyz-encript-cocoscreator/master/screen-shot.png)


Features:
- **web**Support encrypted pictures, Text, JSON
- **native terminal**Support all resources except audio except audio
- Support file name confusion

**Encryption:**
Encryption is the simplest difference or encryption. Modify the constructed source code for decryption.The Native terminal is to modify the file reading function of the CCFileUtil. The web side is the DOWNLOAD series method that modifies the COCOS2D-JSB.JS.

**File name modification thinking:**
Extract the file name and rename the MD5 code of the file name; then before downloading the resource, modify the Transformurl function first,
Calculate the local file name once again MD5 for redirection;

**How to use:**
It must be constructed first. At present, JSB-Link, Web-Mobile, Web-Desktop, and then open the plug-in, select the corresponding and build, fill in the encryption signature, secret key, and click the encryption button.