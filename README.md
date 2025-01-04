# Google Glass In 2025

## What is Google Glass?
Google Glass was a wearable, voice and motion-controlled device that were designed to look like glasses. It displayed information to the users field of vision and was launched in 2013. Some of the features of this device includes: 
- Apps: Twitter, Facebook, Google Hangouts, Google Maps
- Camera: 5 MP photos and 720p video
- Display: A small, transparent display on the right side of the frame
- Input: Voice commands, touchpad, and the MyGlass phone app

## Why Google Glass Failed
There are multiple reasons why Google Glass ended up failing. Although it was a first of its kind technology, it had its flaws. The first reason was that it was marketed as a "luxury" item. With its expensive price of $1,500, the average consumer couldn't afford to buy one. It was designed for those interested in technology and potential investors. Another reason Google Glass failed was that it was considered dangerous. There were many concerns over safety, such as driving while wearing the glasses and not paying attention to your surroundings. Interesting how no one seems to be too worried about that now with phones, Apple Vision Pros, etc. One last reason it failed was its design. To its credit, it definitely looked futurisitic, but to many it seemed to be bulky and ugly.

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

The first step of this process is to verify the device is in fastboot. The serial number of the dervice should show up. If you see the device serial number show up after entering this command, you can continue on with the next step.

![Screenshot 2025-01-01 201220](https://github.com/user-attachments/assets/79510b45-3ff3-4ae3-827a-779a02d74d46)

Now we unlock flashing by using the following command

![Screenshot 2025-01-01 201243](https://github.com/user-attachments/assets/b49f3506-439c-4e3a-8901-bd16bbe8c916)

Now we can flash the device!

![Screenshot 2025-01-01 201304](https://github.com/user-attachments/assets/a7a0c9c2-7d4a-4622-ab96-70d655078f65)
![Screenshot 2025-01-01 201317](https://github.com/user-attachments/assets/dc73cb9c-d8bb-40b5-88ce-1c767fdc3578)
![Screenshot 2025-01-01 201326](https://github.com/user-attachments/assets/42fe9a2d-b116-426a-9504-1572d6f14529)

These next commands are optional, but I want to erase the cache, userdata partition, and re-lock the bootloader

![Screenshot 2025-01-01 201336](https://github.com/user-attachments/assets/5877c09e-0911-41a2-b2f9-d2ed35602e5f)

I can now unplug Google Glass from my computer and use them!

I was looking into the current features that it has, but it is very limited. You can only see the time and take photos/videos with it. Knowing it has limited features, I decided to take some photos around my town and record some videos while I was in New York City! 

## Conclusion
At the time of its release, Google Glass was a special product and a first of its kind. Unfortunately, it didn't change the world like it hoped to. It was a very special device that paved the way for the future of glasses technology. Meta's Ray-Ban has similar features to what Google Glass had, but with full frames and not only seeing a screen in the corner. It was fun learning more about them and using them to record videos during my travels. I learned more about flashing devices and about Android (which is basically what Google Glass is using). Thanks for reading! Stay tuned for more projects coming soon!
