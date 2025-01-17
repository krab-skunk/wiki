# Install Windows 11 24H2 without TPM and Secure Boot requirements

1. Create a Windows 11 ISO with Microsoft's [Media Creation Tool](https://go.microsoft.com/fwlink/?linkid=2156295)
2. Download Rufus and check all the check box, that's it 

# Install Windows 11 24H2 without TPM and Secure Boot requirements

1. Create a Windows 11 ISO with Microsoft's [Media Creation Tool](https://go.microsoft.com/fwlink/?linkid=2156295)
2. Install [Setup Patchium](https://www.iumkit.net/portail/setup-patchium/) and run it
3. Home tab: Select ISO, wait during processing
4. Go to Install > Uncheck Remove upgrade and Check Disable Windows 11 compatibility restrictions, click Apply
5. Optional: To install without a Microsoft account, go to Install OOBE tab. Click Integrate lumOOBE
6. Click on Create ISO button
7. Use Rufus or [Ventoy](https://www.ventoy.net/en/download.html) (prefered) to run installation from a USB drive

## Upgrade Windows 11

1. Download [MediaCreationTool.bat](https://github.com/AveYo/MediaCreationTool.bat/archive/refs/heads/main.zip)
2. Unzip archive and navigate to the `/bypass11` folder.
3. Find the file `Skip_TPM_Check_on_Dynamic_Update.cmd`, select it, right click > Run as Administrator.
4. Then run a mounted Windows 11 installer ISO (See previous chapter or download from [Microsoft](https://www.microsoft.com/fr-fr/software-download/windows11))

Or use [Flyby11](https://www.justgeek.fr/flyby11-installer-windows-11-pc-non-compatible-131069/)

