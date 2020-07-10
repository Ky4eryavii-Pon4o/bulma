---
layout: post
title: Changing Screen Resolution of Mac OS VirtualBox Guest
date: 2020-07-10 07:49:35
---
The default screen resolution for Mac OS X VirtualBox Guest is 1024×768.\
Below shows how to change the screen resolution of Mac OS VirtualBox guest running on Windows 10.


**Steps:**

1. Open “Command Prompt”. (press Win + x and select “Command Prompt”)
2. Navigate to VirtualBox folder in which “VBoxManage.exe” resides.

<code>cd C: \ Program Files \ Oracle \ VirtualBox</code>

3. Set resolution by typing the command below.

<code>VBoxManage setextradata "catalina2019" VBoxInternal2 / EfiGraphicsResolution 1440x900</code>\
The third parameter (i.e. “catalina2019”) should be your VM name.

4. Start the VM