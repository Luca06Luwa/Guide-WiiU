# Unblocking Updates
---
This is needed if you ever need to perform a System Update.

?> If you are running Aroma and have deleted the update folder, you need to disable both autobooting and recreate the update folder.

### Instructions {docsify-ignore}

<!-- tabs:start -->

#### **Removing PayloadLoader Autoboot**

### Removing PayloadLoader Autoboot

?> When autobooting into the PayloadLoader, updates are **NOT ALWAYS** automatically blocked. Follow the guide below to disable it.

1. Boot the console while holding X on the Gamepad.
1. Navigate to the `installer` environment and launch it by pressing A.
1. Press A to select `Check`.
1. Select `Boot options`.
1. You will be asked if you want to switch the boot title. Press A to select `Switch back to Wii U Menu`.
1. When the process finished, press A to shutdown the console.
1. Perform the System Update.
1. Follow [this](../docs/user-guide/aroma/autoboot) to re-enable autobooting.

#### **Recreating Update Folder**

### Recreating Update Folder

1. Plug your SD Card into your Computer.
1. Download and extract [UFDiine](https://github.com/GaryOderNichts/UFDiine/releases/latest) to the root of your SD Card.
1. Plug the SD Card into your Wii U console and power it on.
1. Run the UFDiine app from the Wii U Menu.
1. Press the A button to create the update folder.
1. Confirm that it says `Update folder exists`. You are no longer blocking updates.

#### **Removing DNS Blocks**

### Removing DNS Blocks

1. Enter the Wii U's system settings and navigate to `Internet > Connect to the Internet > Connection List >`
`Your WiFi connection > Change Settings > DNS` and set the option to `Auto-obtain`.
1. You are no longer blocking system updates.

<!-- tabs:end -->
