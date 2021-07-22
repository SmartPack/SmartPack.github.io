---
layout: post
title: Android Rooting
date: February 03, 2021
permalink: /android-rooting/
---

<style>
    tab1 { padding-left: 4em; }
</style>

<h3 style="color: blue">What is Rooting?</h3>

<p style="text-align: justify;"><tab1>Rooting, considered as an illegal activity by most mobile manufacturers (OEMs), is a process of gaining superuser access over the android ecosystem. As you probably know, a Linux system offers superuser (su) rights to advanced users, which makes them capable of doing a whole bunch of tasks that are natively unavailable for normal users. As an operating system using a modified Linux Kernel as a base, android also has the exact same feature, which is, however, disabled by default by all the OEMs on their production builds. It is definitely logical by considering the fact that the superuser power on the hands of a noob user is as dangerous as a virus on a human body. For example, a root user can easily manipulate system properties, or in the worst case can delete some of the essential system files that are not even accessible for normal users.</tab1></p>

<p style="text-align: justify;"><tab1>On the other hand, the superuser privileges on an experienced hand will make them capable to do anything on an android device. Imagine, you bought a latest flagship and your OEM provides your device with a number of nonsense system apps (and so non-removable) that you likely never use in your whole life. Root access will make you capable of removing any system apps, either on a root shell, or by using a suitable third party application. If you are lucky enough with community development support, it is also possible to replace the entire operating system with a custom one made for your device. Thanks to the open source nature of android, the majority of the popular android devices available on the market holds a strong and very active alternate development support, though most of the normal users are either unaware or ignorant of it. The above-mentioned alternate development includes, but not limited to.</tab1></p>
* Custom ROMs (fully replaces the stock firmware)
* Custom Kernels (add useful features to an android device by injecting a modified kernel)
* Various modules to do tasks that are not supported natively by an OEM, etc.

<p style="text-align: justify;"><tab1>Another important scenario is to improve the overall efficiency of an android device, or extend the battery life by tweaking some of the kernel parameters with the help of a powerful kernel manager application, which are also beyond the scope of a non-rooted user. <a href="{{ site.github.url }}/spkm/">SmartPack-Kernel Manager</a> is a good example of this kind.
</tab1></p>

<p style="text-align: justify;"><tab1>Historically, rooting on various android versions is achieved by utilizing one or more of the exploits found on the source code to inject su binary to the /system/bin or /system/xbin directory. The evolution of projects, such as SuperSU and Magisk by community developers makes rooting much easier for most devices. Later, the active development, open source nature, and system-less behaviour of Magisk makes it as the favorite root solution for most root lovers. Moreover, gaining root access on many devices are as simple as sending a few commands on fastboot or flashing a simple zip file.</tab1></p>

<h3 style="color: blue">Advantages of Rooting?</h3>

<p style="text-align: justify;"><tab1>The ultimate control over an android device achieved by rooting offers infinite opportunities to a power user. Some of them are.</tab1></p>
* Replace the entire firmware provided by the device manufacturer with a completely new one. It will open up unique opportunities for users to enjoy latest android releases on their relatively old devices in which the official updates from the respective OEMs are most likely unavailable.
* Use a kernel manager to manipulate kernel parameters for an improved performance or extend battery life (better user experience in general).
* It is even possible to replace the stock kernel provided by an OEM with a custom one to achieve more kernel-level features.
* Easily remove unwanted system applications, either in command-line or by using a third party application (e.g. <a href="https://smartpack.github.io/PackageManager/" target="_blank">Package Manager</a>, <a href="https://sunilpaulmathew.github.io/De-Bloater/" target="_blank">De-Bloater</a>, etc).
* Customize almost every part of an android device (example: a custom boot screen).
* Installing an OEM specific application on a device made by another OEM.
* Installing a Magisk or Xposed modules to bring the customization on your device into another level.
* Many more

<h3 style="color: blue">Disadvantages of Rooting?</h3>

<p style="text-align: justify;"><tab1>Rooting will give a user the ultimate power on an android device. This is, however, totally against the normal behavior of a Linux-based eco-system as rooting allows a user to interact with the top-level system files or data files owned by other users. The above mentioned restrictions to access the system properties as well as other user’s data files played an important role to make a Linux based operating system as safe as it is today. As a result, it is very likely that a malicious software installed on a rooted device silently steals or manipulates the sensitive data of a noble user. As an example, an application enjoying root privileges can read and write almost any part of an android device’s storage even on modern devices, whereas a normal user application requires storage write permission to be granted by individual users, provided the device is running on Android 6 (Marshmallow) or above.</tab1></p>


<p style="text-align: justify;"><tab1>Also, accidental or intentional removal of some of the system properties will leave an android device completely useless, either temporarily or permanently in the worst scenario. It is also worth mentioning that a number of popular android applications, especially banking and other online payment interfaces may not work on rooted devices due to the restrictions imposed by their developers. Moreover, boot loader unlocking, an essential process that should be done to gain root access on most modern devices, will certainly void the manufacturer’s warranty.</tab1></p>

<hr>

<h4>This is a part of an article originally published by <a href="https://play.google.com/store/apps/dev?id=5836199813143882901" target="_blank">sunilpaulmathew</a> on <a href="https://arenaoftech.com/" target="_blank">https://arenaoftech.com/</a>. The original article is available <a href="https://arenaoftech.com/post/android-rooting-pros-and-cons/" target="_blank">here</a>.</h4>
