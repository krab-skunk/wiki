I have had this issue on 24H2, and the fix was not as simple as the comments below suggest. The machine is registered to an org that no longer needs the machine, i cannot ask them to remove it from intune. OOBE\BYPASSNRO would not work, I tried all sorts of things but no option was given to continue without network.
What worked in the end was forcing an install of the home edition. This is not as trivial as it sounds as M$ don't provide individual ISOs for versions anymore. So I followed the below steps:
1. Create a Win11 USB key with Rufus or Windows 11 media creation tool
2. Go to this website: https://schneegans.de/windows/unattend-generator/
3. Fill out how you want your Windows to be setup. Importantly, on Windows Edition choose 'use generic key' and select 'Home' edition.
4. Scroll to the bottom and download the XML file
5. Place the autounattend.xml on the root of the install USB
6. Plug in an install windows as normal
Caveats - you will need to use a MS account as this is required for Home editions. You could use a burner account to get past this, then upgrade your version of Windows to Pro from the settings screen and then create a local account, but I didn't try this
Hope this helps someone

https://www.reddit.com/r/Intune/comments/1cto1ed/comment/ly9jqdi/?utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button

https://schneegans.de/windows/unattend-generator/

——
https://answers.microsoft.com/en-us/insider/forum/all/set-up-windows-11-without-internet-oobebypassnro/4fc44554-b416-4ecb-8961-6f79fd55ae0f

Press Shift + F10. The command prompt opens 
 
net.exe user "User Name" /add 
 
net.exe localgroup "Administrators" "User Name" /add 
 
cd OOBE 
 
msoobe.exe && shutdown.exe -r 
 
Windows will now restart and start with the other settings until Windows 11 is installed correctly with a local account. 
  
When logging in, "The user name or password is incorrect" now appears. 
 
Simply press OK and select the right account at the bottom left of screen. You should have one for Administrator and one for whatever name you used as "User Name" above.
