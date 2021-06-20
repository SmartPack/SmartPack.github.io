---
layout: default
title: Kernel Downloads
permalink: /kerneldownloads/
---

<style>
    tab1 { padding-left: 4em; }
</style>

<h2 style="color: red; text-align: center">Kernel Downloads</h2>

<h3 style="color: blue">Introduction</h3>
<p style="text-align: justify"><tab1>This feature will basically allow a developer to add kernel downloads, and auto-flash (not for all devices) support to any Kernel's available for a device through SmartPack-Kernel Manager. The only requirement is to host a "<b>.json</b>" file with kernel specific data on somewhere in the web. The json file should be updated upon each and every kernel release. The app will automatically acquire the data from the json file once in every 24 hr (configurable) and display the latest version information within the app. This feature is inspired from a similar feature in <b>franciscofranco</b>'s <b>FK-Kernel Manager</b> (huge thanks to him for the original idea). Hence, the json files created for FK-Kernel Manager will simply work here as well.</tab1></p>

<hr>

<h3 style="color: blue">How-to Create an Update Channel (for <i>Developers</i>)</h3>

* Download the model json file from <a href="https://raw.githubusercontent.com/SmartPack/SmartPack.github.io/master/asset/kernel-downloads.json" target="_blank">here</a>
* Properly update the following entries in the json
  * Replace "<b>Kernel_Name</b>" with the name of your kernel.
  * Replace "<b>download_link</b>" with the direct download link to the latest version of your kernel. <b>Please note</b>: The provided link should be capable to download the kernel zip in one click.
  * Replace "<b>changelog_url</b>" with the latest change-logs of your kernel. <b>Please note</b>: You can either paste the change logs in a well aligned format, or give a link to reach the same.
  * Replace "<b>sha1</b>" with the sha1 of your latest kernel. It will be evaluated by the app to make sure the authenticity of the downloaded zip file. <b>Please note</b>: sha1 is optional, but highly recommended. Also, if you decided to provide sha1, please make sure that it is accurate to avoid download failure message from the app.
  * Replace "<b>support_link</b>" with a link to any support thread (e.g. xda) or group (e.g. Telegram) available for your kernel.
  * Optionally, you can also add a "<b>donation_link</b>", which will be also shown within the app.
* Host this file on somewhere (e.g. GitHub) and give a direct download link of the same to your users.

<hr>

<h3 style="color: blue">How-to import an Update Channel (for <i>Users</i>)</h3>

* Simply open the app, go to SmartPack page, and input the link provided by your kernel developer in the <b>Update Channel</b> menu.

<hr>

<h3 style="color: blue">How-to remove/replace an Update Channel (for <i>Users</i>)</h3>

* Simply clear/or replace the link added to the <b>Update Channel</b> menu.
