---
layout: post
title: ADB De-bloating
date: February 26, 2021
permalink: /adb-debloating/
---

<style>
    tab1 { padding-left: 4em; }
</style>

<h3 style="color: blue">De-bloating with ADB</h3>

<p style="text-align: justify;"><tab1><b>De-Bloating</b>, the process of removing bloatwares (general terminology used to represent unwanted applications pre-installed on an android device by the manufacturer or carrier) from a device shall be done on non-rooted devices by utilizing the power of <b>Android Debug Bridge</b> (<b>ADB</b>). Most majority of android users, however, blindly believe that the tools like ADB are designed only for developers, but not for common people. Although ADB tools are much useful for developers to debug their applications and more, this method also offers some advanced control over an android device for normal users via its powerful command-line interface. Other than a one-time configuration process that likely causes some headache to beginners, doing some basic tasks on ADB is not at all a difficult task. The sole intention of this article is to help users to properly configure a working ADB environment and conduct some basic de-bloating tasks. If you're an advanced user who is already using a rooted device, you can probably move to our other guide (<a href="{{ site.github.url }}/debloating/">De-bloating</a>), which is solely written for rooted devices. The merits and demerits of rooting an android device is also explained in one of our articles (<a href="{{ site.github.url }}/android-rooting/">Android Rooting</a>).</tab1></p>

<h3 style="color: blue">What is Android Debug Bridge (ADB)?</h3>

<p style="text-align: justify;"><tab1>Android Debug Bridge (ADB) is a versatile command-line tool allowing advanced users to communicate with an android device. The ADB command facilitates a variety of device actions, such as installing and debugging apps, and it provides access to a Unix shell that can be used to run a variety of commands on a device. A much more detailed information on ADB and the usage of its command line tool are available <a href="https://developer.android.com/studio/command-line/adb">here</a>.</tab1></p>

<h3 style="color: blue">What are the requirements for ADB De-bloating?</h3>

* A Computer or Laptop (Windows/Linux/Mac)
* A USB cable to connect your android device with computer

<h3 style="color: blue">How to configure Android Debug Bridge (ADB)?</h3>

* Download and Install OEM specific USB drivers from <a href="https://developer.android.com/studio/run/oem-usb">here</a>.
* Download the ADB binary for your OS (Windows, Mac, Linux) from <a href="https://developer.android.com/studio/releases/platform-tools">here</a> and extract the zip file into a folder that you can quickly access.
* On your phone, go to <b>Settings</b> --> <b>About Phone</b> and tap on the "<b>Build number</b>" at least 7 times to enable the "<b>Developer Options</b>".
* Now find and navigate to the newly enabled "<b>Developer Options</b>" from the "<b>Setting</b>" and find "<b>USB Debugging</b>". Enable it.
* Plug your phone into the computer via USB cable.
* On your computer, browse to the directory where you extracted the ADB binary in step 2.
* Launch <b>Command Prompt</b> (Windows) or <b>Terminal/Shell</b> (Linux/Mac) in your ADB folder.
* Enter the following command:<br>"<b>adb devices</b>"<br>You will see that the system is starting the ADB daemon. Also, you will probably see a prompt on your phone asking you to authorize a connection with the computer. Grant it. If you re-run the "<b>adb devices</b>" command, the terminal will print the serial number of your device, meaning your mobile is successfully connected to the computer via ADB.
* Now sending the following command from the Command Prompt/Terminal/Shell will remove the system application of your choice.

<h4 style="color: red">"adb shell pm uninstall -k --user 0 package_id"</h4>

<p style="text-align: justify;"><tab1>where “<b>package_id</b>” is the unique application id of the bloatware you want to remove. Please be aware that the “<b>package_id</b>” of an android application, which looks like a java package name, such as “<b>com.example.bloatware</b>”, is most likely different to that of the application name.</tab1></p>

<p style="text-align: justify;"><tab1>For example, to uninstall Google Chrome from a device using this method, a user needs to execute the following command.</tab1></p>

<h4 style="color: red">adb shell pm uninstall -k --user 0 com.android.chrome</h4>

<p style="text-align: justify;"><tab1>Also, please do remember to checkout the official documentation of <a href="https://developer.android.com/studio/command-line/adb">ADB</a>, where a whole list of command line tasks are listed with proper examples. Cheers.</tab1></p>