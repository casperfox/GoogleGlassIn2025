# Google Glass In 2025

## Introduction


## What is Google Glass?


## My Experience
Back in 2022, I was given Google Glasses and didn't know much about them. Google Glasses had plenty of great features and was outstanding during that time. I wanted to see what features I could use with the current version installed on the device today, in 2025.

![IMG_8006_2000x1958](https://github.com/user-attachments/assets/1fcdc75f-fb6a-4de3-9dc2-b5e0c3471884)

When I first turned it on and went through the tutorial that it had for new users, I ran into a huge problem. I needed to sign into my google account through the Google Glasses using a website link/QR code provided, but that link no longer exists, as they discontinued the Google Glass project years ago.

I sat and thought about ways to get past this problem and had to do some research to figure out what to do. Based on what I could find online, the only way to use the device without signing in would be to factory reset the device, reboot it into fastboot, and install the final software update on it. To get a copy of the final software update, Google provides a tutorial on downloading the required files and how to flash the update to the device. You can find the article 
[here.](https://support.google.com/glass/answer/9649198?hl=en)

After downloading the final software update and finding the platform-tools they provide, I now had to boot my Google Glass into recovery mode. To boot into recovery mode, the method of holding down the camera button then pressing the power button and continuing to hold the camera button for 10 seconds worked for me. Once in recovery mode, you simply have to select the option to reboot your device into fastboot. Then I plug in my Google Glass to my computer and start up command prompt in the developer-tools directory.

This is where things became challenging for me. When I plugged in my Google Glass, there were driver issues causing the developer-tools to not detect the device plugged in. For some reason, Windows 11 couldn't recognize the device and I couldn't use the developer-tools to flash the device with the software update.

![Screenshot 2025-01-02 211205](https://github.com/user-attachments/assets/73e312eb-8468-4436-a63b-f4119bcdca50)

After doing some research, I found the correct driver I needed for this to work. I downloaded the Google USB Driver from [here](https://developer.android.com/studio/run/win-usb), and installed it onto my computer.

![Screenshot (3)](https://github.com/user-attachments/assets/ca190fd8-6e41-4688-99bd-a770a2a05513)

Once it was installed, I then had to update the glass_1 driver, browse for drivers on your computer, and then pick from a list of available drivers. I selected the newly installed driver, Android ADB Interface, and now I can start the flashing process.

![Screenshot 2025-01-01 201613](https://github.com/user-attachments/assets/10f706aa-c7b4-483a-806e-4fcc2b05c162)


## Conclusion

