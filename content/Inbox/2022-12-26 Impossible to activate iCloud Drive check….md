---
title: "2022-12-26 Impossible to activate iCloud Drive check…"
---


[[- ReadItLater]] [[- Article]] [[- InternetScrap]]

# [Impossible to activate iCloud Drive check…](https://discussions.apple.com/thread/252781437)

Looks like no one’s replied in a while. To start the conversation again, simply [ask a new question.](https://discussions.apple.com/post/question?communityId=2877020)

Windows 10 Pro, 20H2, 19042.985

iCloud 12.3

Each time I activate iCloud Drive checkbox and press Apply button – checkbox deactivates automatically. Earlier iCloud Drive worked OK. Any ideas how to fix this?

Windows, Windows 10

Posted on May 19, 2021 2:03 AM

7 replies

[May 20, 2021 6:03 AM in response to Zam\_vr\_](https://discussions.apple.com/thread/252781437?answerId=252781437021#252781437021)

Hi Zam\_vr\_,

Thank you for using the Apple Support Communities. We understand that the iCloud Drive in the iCloud for Windows app is not activating and we are happy to help!  Follow the troubleshooting steps in the articles below and check to see if the issue is still there after each one:  

1.  [Restart (reboot) your PC](https://support.microsoft.com/windows/restart-reboot-your-pc-110262aa-fc79-1c33-7b00-c140ae3a6dac)
2.  [Update Windows 10](https://support.microsoft.com/windows/update-windows-10-3c5ae7fc-9fb6-9af1-1984-b5e0412c556a)
3.  Make sure TCP ports are open: [TCP and UDP ports used by Apple software products](https://support.apple.com/HT202944)
4.  Uninstall security software: [Resolve issues between iTunes and third-party security software](https://support.apple.com/HT201413)

We hope this helps! 

Take care

[May 20, 2021 6:03 AM in response to Zam\_vr\_](https://discussions.apple.com/thread/252781437?answerId=252781437021#252781437021)

Hi Zam\_vr\_,

Thank you for using the Apple Support Communities. We understand that the iCloud Drive in the iCloud for Windows app is not activating and we are happy to help!  Follow the troubleshooting steps in the articles below and check to see if the issue is still there after each one:  

1.  [Restart (reboot) your PC](https://support.microsoft.com/windows/restart-reboot-your-pc-110262aa-fc79-1c33-7b00-c140ae3a6dac)
2.  [Update Windows 10](https://support.microsoft.com/windows/update-windows-10-3c5ae7fc-9fb6-9af1-1984-b5e0412c556a)
3.  Make sure TCP ports are open: [TCP and UDP ports used by Apple software products](https://support.apple.com/HT202944)
4.  Uninstall security software: [Resolve issues between iTunes and third-party security software](https://support.apple.com/HT201413)

We hope this helps! 

Take care

[May 20, 2021 6:26 AM in response to i\_rina](https://discussions.apple.com/thread/252781437?answerId=255241302022#255241302022)

Hi i\_rina.

My current Windows version is the last one, so I can't update it further.

iCloud ports are open.

Third-party security software is absent. I use only native Windows Defender.

[May 20, 2021 7:12 AM in response to Zam\_vr\_](https://discussions.apple.com/thread/252781437?answerId=252781437021#252781437021)

Zam\_vr\_,

If you have followed all the steps in the Apple Support articles and iCloud Drive is still not activating, then we recommend that you [Contact - Official Apple Support](https://support.apple.com/contact).

Have a good day!

[May 23, 2021 6:32 AM in response to Jeff\_W.](https://discussions.apple.com/thread/252781437?answerId=255241637022#255241637022)

An update on my problem. Here is what iCloud log files returns:

ERROR RunCloudDocs Error launching: iCloudDrive-AppX.exe enable: 2

ERROR CloudDocsService::SaveSetting Failed to enable

[Jun 7, 2021 8:02 AM in response to Zam\_vr\_](https://discussions.apple.com/thread/252781437?answerId=255257558022#255257558022)

Hi Zam\_vr\_,

Have you found a solution o you issue because i experiment the same issue execpt i 'm on 21H2 windows 10 version and logs are the same

[Jun 7, 2021 8:22 AM in response to asimov67](https://discussions.apple.com/thread/252781437?answerId=255344460022#255344460022)

Hi, asimov67.

I guess that this problem is connected somehow with the fact that I worked under domain user.

In the end I was able to activate iCloud Drive but here is how my experience looked like:

1.  I reinstalled Windows.
2.  I created a local Windows user and installed iCloud.
3.  After several hours it stopped working (logs were the same), so i moved to domain user (provided by my work administrator).
4.  I installed iCloud again and it works properly.

-   [](https://discussions.apple.com/thread/252781437?page=1)
-   
-   of 1
-   
-   [](https://discussions.apple.com/thread/252781437?page=1)

Impossible to activate iCloud Drive checkbox