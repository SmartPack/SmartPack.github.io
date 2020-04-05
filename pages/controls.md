---
layout: smartpack
title: Custom Controls
permalink: /spkm/customcontrols/
---

<style>
    tab1 { padding-left: 4em; }
</style>

<h2 style="color: red; text-align: center">Custom Controls</h2>

<h3 style="color: blue">DISCLAIMER</h3>
<p style="color: red; text-align: justify"><b>This feature is too powerful to mess your device. If you are unsure about something, better do not play with it. And as always,<br><br>**USE AT YOUR OWN RISK**</b></p>

<p style="text-align: justify">Currently, the custom controls feature on SmrtPack-Kernel Manager offeres the creation of two different types of controllers, and are</p>
* a classical Switch item for boolean sysfs paths having values 0 or N (disable) and 1 or Y (enable)
* a more generalised Input-type item, which should work with any sysfs path having any value

<h3 style="color: blue">How to add a controller</h3>

<p style="text-align: justify">There are two different ways to create a custom controller on SmrtPack-Kernel Manager, and are</p>
* <i>For normal users</i>: Open the app, move to <b>Custom Controls</b>, click the "<b>plus</b>" icon, select the desired option and simply pick the sysfs path from <b>/sys</b> (or any other) folder using a supported <b>Root File Manager</b>. The only need to get this way working is the availability of a supported <b>Root File Manager</b> installed on the device. Some of the supported File Managers includes
  * <b><a href="https://play.google.com/store/apps/details?id=me.zhanghai.android.files&hl=en" target="_blank">Material Files</a></b>
  * <b><a href="https://play.google.com/store/apps/details?id=fm.clean.pro" target="_blank">File Manger for Superusers</a></b>
  * <b><a href="https://play.google.com/store/apps/details?id=com.jrummy.root.browserfree&hl=en" target="_blank">File Explorer Root Browser</a></b>
* <i>For advanced users</i>: Save the sysfs path you wish to add into a text file and place inside <b>/sdcard/SP/controls/switch/</b> (for creating a switch item) or <b>/sdcard/SP/controls/generic/</b> (for creating a generic input item). The text file (without the "<b>.txt</b>" extension) might be saved by any name.

<hr>

<h3 style="color: blue">How to remove a controller</h3>

<p style="text-align: justify">Click the Pop-Up menu on the right bottom corner of each controller, and select the delete option. Alternatively, go to <b>/sdcard/SP/controls/switch/</b> (for removing a switch item) or <b>/sdcard/SP/controls/generic/</b> (for removing a generic input item) and simply delete the respective file.</p>
