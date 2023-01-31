# Aroma {docsify-ignore-all}

## Finalizing Setup

Now that PayloadLoader, Environment Loader and Aroma are installed, we are going to finalize the setup.

We are going to make the Aroma environment start automatically when your console autoboots the Health and Safety Information app (or when manually launching it if you chose not to autoboot it) and select Wii U Menu as default as well as getting additional homebrew apps.

### Setting up PayloadLoader, Environment Loader and Aroma

1. Turn on your Wii U.
    - The Environment Loader should show up.
1. Using the D-Pad, navigate to `aroma` and press Y to set this to your default envrionment, then press A to launch into Aroma.
    - You might get a red warning screen telling you that updates aren't blocked properly. Press A to continue anyway. We're going to block updates in the "Blocking Updates" section below.
    - To open the Environment Loader in the future, you have to hold X while your Wii U is booting up.
1. On the Aroma Boot Selector, the `Wii U Menu` should already be selected, press Y to set this to your default autobooting option, then press A to launch into the Wii U Menu.
    - To open the Aroma Boot Selector in the future, you have hold START (+) while your Wii U is booting up.

?> Once you're booted into the Aroma environment, you can launch homebrew at any time by launching it from the Wii U Menu.

### Blocking Updates
While Aroma's PayloadLoader already has built-in update blocking functionality, it is recommended to delete the update folder to effectively block system updates.
If you get a red warning screen while booting into Aroma, the update folder still exists and it is recommended to delete it using [this guide](../block-updates).

You are now running Aroma. Any apps you have on your SD Card will show up on the Wii U menu.

?> **Aroma does not support the Homebrew Launcher**  
Launch apps from the Wii U menu using the `homebrew_on_menu` plugin.

You can now open the Plugin Configuration Menu using `L + Down + SELECT (-)` on the GamePad or Pro Controller (or `B + Down + Minus (-)` for WiiMotes).

### Installing apps, modules, and plugins

Base-Aroma already comes with several useful plugins and modules.  
You can also install additional Aroma compatible apps, modules and plugins. Below is a list with various recommendations.

| Name | Description | Installation Instructions |
| ---- | ----------- | ------------ |
| [Save Mii Mod WUT Port](https://github.com/Xpl0itU/savemii) ([Download](https://github.com/Xpl0itU/savemii/releases)) | Lets you manage your Wii U and vWii save data. | 1. Extract the downloaded `SaveMiiModWUTPort-Aroma.zip` file. 2. Copy the `wiiu` folder to the root of the SD Card. |
| [Homebrew Appstore](https://github.com/fortheusers/hb-appstore) ([Download](https://github.com/fortheusers/hb-appstore/releases)) | Lets you browse and download homebrew apps directly from your Wii U. | 1. Extract the downloaded `wiiu-extracttosd.zip` file. 2. Copy the `wiiu` folder to the root of the SD Card. |
| [FTPiiU Plugin](https://github.com/wiiu-env/ftpiiu_plugin/) ([Download](https://github.com/wiiu-env/ftpiiu_plugin/releases)) | Runs a FTP server in the background. | 1. Extract the downloaded `ftpiiu_vX_X.zip` file. <br> 2. Copy the `ftpiiu.wps` to the `wiiu/environments/aroma/plugins` folder on the root of your SD Card. |
| [SDCafiine](https://github.com/wiiu-env/sdcafiine_plugin/) ([Download](https://github.com/wiiu-env/sdcafiine_plugin/releases)) | Allows you to mod games by redirecting files to the SD Card. | 1. Extract the downloaded `sdcafiine_vX_X_X.zip` file. <br> 2. Copy the `sdcafiine.wps` to the `wiiu/environments/aroma/plugins` folder on the root of your SD Card. |
| [Bloopair](https://github.com/GaryOderNichts/Bloopair/) ([Download](https://github.com/GaryOderNichts/Bloopair/releases)) | Allows wirelessly connecting most popular Bluetooth capable controllers. | 1. Extract the contents of the newly downloaded `Bloopair_vX.X.X.zip` file. <br> 2. Copy the `30_bloopair.rpx` to the `wiiu/environments/aroma/modules/setup/` folder on the root of your SD Card. <br> 3. Copy the `wiiu` folder to the root of your SD Card. |
| [Screenshot Plugin](https://github.com/wiiu-env/ScreenshotWUPS/) ([Download](https://github.com/wiiu-env/ScreenshotWUPS/releases)) | Allows taking screenshots directly to the SD Card. | 1. Extract the downloaded `screenshot_plugin_vX_X.zip` file. <br> 2. Copy the `screenshot.wps` to the `wiiu/environments/aroma/plugins` folder on the root of your SD Card. |

### Using Tiramisu (Fallback)

Tiramisu is used when installing aroma and can be used as a fallback if aroma isn't working well.
To switch to tiramisu, simply follow these steps:

1. Take the SD Card out of your computer and plug it into your Wii U console.
1. Start the EnvironmentLoader.
    - If you're autobooting into it, this can be done by powering on your console and holding `X`.
1. Highlight the entry called `tiramisu` using the D-Pad.  
    - To make the console autoboot Tiramisu press `Y`.
1. Launch Tiramisu by pressing `A`.
