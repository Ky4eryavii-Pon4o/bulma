---
layout: post
title: Enable new Start Menu on Windows 10 v2004
date: 2020-08-14 11:40:16
---
> Но прежде убедитесь, что вы установили сборку 19041.423 на свой компьютер с Windows 10. Вы можете получить соответствующий номер сборки, загрузив и установив предварительный патч KB4568831 из каталога Центра обновления Майкрософт.

To enable the new [Windows 10 Start menu](https://www.thewindowsclub.com/customize-start-menu-in-windows-10) using Registry Editor, follow the below instructions. But before you begin, [create a system restore point](https://www.thewindowsclub.com/create-system-restore-point) first.

Before you start the procedure, make sure the OS version of your Windows raises to Build 19042.423 or higher. In case you have the earlier version of the operating system, get it by *[navigating to Settings](https://www.thewindowsclub.com/windows-10-settings) > Windows Update*. On moving to the right pane, click *Check for updates* > *View optional updates* link, and then install the build.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Now open the Run dialog box using *Win+R* keyboard shortcut.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

In the text field, type *regedit* and hit enter.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

If you’re prompted by User Account Control, click *Yes* to provide the grant privileges.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

In the Registry Editor window, go to the following path:

<!-- /wp:paragraph -->

<!-- wp:preformatted -->

```

```

<!-- /wp:preformatted -->

<!-- wp:image {"align":"center","id":224626} -->

![Enable the new Start Menu on Windows 10 version 2004](https://www.thewindowsclub.com/wp-content/uploads/2020/08/Enable-the-new-Start-Menu-on-Windows-10-version-2004.png "Enable the new Start Menu on Windows 10 version 2004")

<!-- /wp:image -->

<!-- wp:paragraph -->

In the left panel, right-click on the *Overrides* folder and select *New > Key*. Name the new key as **0** and then hit Enter to save it.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Now right-click on the folder named *0* and select *New > Key*. Name the new key as **2093230218** and hit Enter to save it.https://googleads.g.doubleclick.net/pagead/ads?client=ca-pub-5950002284129980&output=html&h=280&slotname=6640627966&adk=485515363&adf=3598821624&w=750&fwrn=4&fwrnh=100&lmt=1597393537&rafmt=3&psa=1&guci=2.2.0.0.2.2.0.0&format=750x280&url=https%3A%2F%2Fwww.thewindowsclub.com%2Fenable-the-new-start-menu-on-windows-10-v2004&flash=0&fwr=0&rpe=1&resp_fmts=1&wgl=1&dt=1597393537383&bpp=4&bdt=187&idt=87&shv=r20200810&cbv=r20190131&ptt=9&saldr=aa&abxe=1&cookie=ID%3Db489f97e3ecaccb7%3AT%3D1597393448%3AS%3DALNI_MaryImmeqOm96LZ2fbxNQh4TjjGPA&prev_fmts=1140x280&correlator=8539998304092&frm=20&pv=1&ga_vid=161375183.1597393449&ga_sid=1597393537&ga_hid=1297870221&ga_fc=0&iag=0&icsg=2288296&dssz=18&mdo=0&mso=0&u_tz=180&u_his=12&u_java=0&u_h=1080&u_w=1920&u_ah=1050&u_aw=1920&u_cd=24&u_nplug=3&u_nmime=4&adx=382&ady=2937&biw=1903&bih=947&scr_x=0&scr_y=0&eid=42530557%2C42530559%2C21066358%2C21066897&oid=3&pvsid=30242788230533&pem=837&ref=https%3A%2F%2Fwww.thewindowsclub.com%2Fpage%2F2&rx=0&eae=0&fc=640&brdim=0%2C0%2C0%2C0%2C1920%2C0%2C1920%2C1050%2C1920%2C947&vis=1&rsz=%7C%7CeEbr%7C&abl=CS&pfx=0&fu=8320&bc=31&ifi=2&uci=a!2&btvi=1&fsb=1&xpc=yvTuul6G9f&p=https%3A//www.thewindowsclub.com&dtd=93

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Next, right-click on the *2093230218* folder and select *New > DWORD (32-bit) Value*. In the right pane, name the new key **EnabledState** and hit Enter.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Finally, double click on the *EnabledState* key to modify it. In the popup menu, set the value data **2** and then click the *OK* button.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Again right-click on the 2093230218 folder and select *New > DWORD (32-bit) Value*. Name the new key as *EnabledStateOptions* and hit enter to save it.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Next, set the Value data 0 like it is already there, and click OK to save it.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Finally, restart your computer to apply the changes.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

After the system reboots, you should now have the new Start menu design with tiles.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

In case there are no such changes in the Start menu, again restart your device or repeat the registry hack.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

You may also save the following code in a **Notepad** and then use it to add the values to your Registry.

<!-- /wp:paragraph -->

<!-- wp:image {"align":"center","id":224652} -->

![new Start Menu on Windows 10 version 2004](https://www.thewindowsclub.com/wp-content/uploads/2020/08/Enable-the-new-Start-Menu-on-Windows-10-version-2004..png "new Start Menu on Windows 10 version 2004")

<!-- /wp:image -->

<!-- wp:paragraph -->

Press *Win+Q* and type *[Notepad](https://www.thewindowsclub.com/basic-notepad-tips)* in the text field. Select the result from the search result to open it.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

In the Notepad window, copy and paste the following syntax:

<!-- /wp:paragraph -->

<!-- wp:preformatted -->

```

```

<!-- /wp:preformatted -->

<!-- wp:paragraph -->

Click *File > Save as* and then save the text file with the .reg file extension, such as *Start Menu.reg*.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Now run this file by double-click on it.

<!-- /wp:paragraph -->

<!-- wp:paragraph -->

Restart your computer to apply the changes.

<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->

#### Restore Windows 10 to existing Start Menu

<!-- /wp:heading -->

<!-- wp:paragraph -->

If you ever would need to get back the changes you made, open the registry editor and navigate to the following path.

<!-- /wp:paragraph -->

<!-- wp:preformatted -->

```

```

<!-- /wp:preformatted -->

<!-- wp:paragraph -->

Now in the left pane, right-click on the *0* folder and select the *Delete* option. Then click on *Yes* to delete the key and all of its subkeys.

<!-- /wp:paragraph -->

<!--EndFragment-->