## RSAT (Remote Server Administration Tools)

RSAT allows IT administrators to manage Windows Server roles and features remotely from a computer running Windows 10 or Windows 7 Service Pack 1.

## Introduction

RSAT cannot be installed on Home or Standard editions of Windows. It is only compatible with Professional or Enterprise editions of the Windows client OS. Unless the download page explicitly mentions that RSAT supports a beta, preview, or other prerelease version, a full (RTM) version of Windows is required to install and use RSAT. Some users have attempted to bypass these restrictions by manually modifying the RSAT MSU to install it on unsupported editions, which constitutes a violation of the Windows end-user license agreement.

Installing RSAT resembles the process of installing Adminpak.msi on Windows 2000 or Windows XP client computers. A key difference is that, in Windows 7, tools do not become available automatically after installation. You need to activate the desired tools through the Control Panel. Navigate to **Start** > **Control Panel** > **Programs and Features**, then select **Turn Windows features on or off** to enable them.

In RSAT releases for Windows 10, all tools are enabled by default. You can open **Turn Windows features on or off** if you wish to disable tools you do not intend to use.

For Windows 7 RSAT, you must enable the specific tools for the roles and features you plan to manage after completing the installation package.

If you need management tools for Windows Server 2012 R2 to manage roles or features on remote servers, no additional software installation is necessary. Launch the Add Roles and Features Wizard in Windows Server 2012 R2 or later. On the **Select Features** page, expand **Remote Server Administration Tools**, choose the desired tools, and complete the wizard to install them.

## RSAT for Windows 10, version 1809 or later versions

> **Note**
> The Turn Windows features on and off dialog in Control Panel is no longer used.

Installing RSAT on Windows 10 version 1809 and later differs slightly from previous versions. RSAT is now integrated into the OS and is added via **Optional Features**.

To enable the tools, navigate to **Start** > **Settings** > **Apps** (for Windows 10 version 22H2 or later, select **System** instead), then choose **Optional features**. Click **Add a feature** and type *Remote* in the search bar to find and enable the RSAT components you need.
