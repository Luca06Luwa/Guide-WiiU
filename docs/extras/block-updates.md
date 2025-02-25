# Blocking Updates
---
All currently known Wii U exploits can, unlike e.g. the Nintendo Switch RCM exploit, be patched by a system update. Although the Wii U is no longer officially supported, Nintendo may still release updates for it. Namely, the updates 5.5.3 up to 5.5.6 were all released after the Wii U was discontinued, so blocking updates is still a recommended action.

While Aroma's PayloadLoader already has built-in update blocking functionality, it is recommended to delete the update folder to effectively block system updates.
If you get a red warning screen while booting into Aroma, the update folder still exists and it is recommended to delete it using the guide below.

### Instructions {docsify-ignore}

Currently, two ways exist to effectively block updates on the Wii U system:
<!-- tabs:start -->

#### **Deleting Update Folder**

### Deleting Update Folder

?> This method is the easier method that is recommended to less advanced users and uses a homebrew app to modify system files. Unlike DNS Blocking, it has the advantage that the eShop's functionality will not be restricted.
1. Plug your SD Card into your Computer.
1. Download and extract [UFDiine](https://github.com/GaryOderNichts/UFDiine/releases/latest) to the root of your SD Card.
1. Plug the SD Card into your Wii U console and power it on.
1. Run the UFDiine app from the Wii U Menu.
1. Press the A button to delete the update folder.
1. Confirm that it says `Update folder is deleted`. You are now blocking updates.

#### **DNS Blocking**

### DNS Blocking

?> This method of update blocking is a bit more advanced than deleting a system file, however, it does prevent the eShop from working. (Basically it just blocks the Nintendo spdate servers). This can be worked around by running [NNUPatcher](https://wiiubru.com/appstore/zips/nnupatcher.zip) before starting the eShop.
1. Plug your SD Card into your Computer.
1. Copy the contents of the `nnupatcher.zip` file to the root of your SD Card. If asked, overwrite any duplicate files.
1. Plug the SD Card into your Wii U console and power it on.
1. Enter the Wii U's system settings and navigate to `Internet > Connect to the Internet > Connection List >`
`Your WiFi connection > Change Settings > DNS` and set the option to `Do not auto-obtain`.
1. You will be asked to input a primary and secondary DNS. Enter the following IP addresses:
    - Primary DNS: 168.235.092.108
    - Secondary DNS: 081.004.127.020
<img src="docs/assets/img/DNS.png" alt="DNS Block">
1. Click on confirm.
1. You are now blocking updates. In order to access the eShop, run the NNUPatcher app from the Wii U Menu before launching the eShop.

<!-- tabs:end -->
