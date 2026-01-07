# at-cmdOS

		AT-CMD By Retromelon

	   Thanks for trying it out ! :)

Download it here : https://payhip.com/b/rjyWc

P.S. - You also need Chrome on your Computer\Laptop to use the Internet.
	   If you accounter problems, send me a message.
	   If you wanna test or modify it feel free to do so ! :)
	   Just make sure to send me a message...

    Make sure that you placed the BatchOS Folder in your Local Disk C://



==================== ABOUT AT-CMD ====================



Developer : Retromelon

Version  : 1.0 Release 1.0

Year    : 2000-2026

Company  : Retromelon's TOYZ Ltd.

Website  : https://retromelon.toyz

License  : Proprietary / All rights reserved



Description:

AT-CMD is a custom batch-based interface that simulates

an operating system environment inside the Windows CMD.

It provides tools like Internet, File Explorer, Task Manager,

System Status, Power Options, and more.



=====================================================

           IMPORTANT

=====================================================



This document explains how to safely replace Windows Explorer (explorer.exe)

with your custom shell (BOOT.exe) for AT-CMD.



Follow these instructions carefully.



-----------------------------------------------------

STEP 1: Open Registry Editor

-----------------------------------------------------

1. Press Win + R to open the Run dialog.

2. Type: regedit

3. Press Enter or click OK.



-----------------------------------------------------

STEP 2: Navigate to the Shell Key

-----------------------------------------------------

For the current user only (recommended):



HKEY_CURRENT_USER\Software\Microsoft\Windows NT\CurrentVersion\Winlogon



For all users (system-wide, NOT recommended):



HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\Winlogon



-----------------------------------------------------

STEP 3: Change the Shell

-----------------------------------------------------

1. In the right pane, locate the value named: Shell

2. By default, it is: explorer.exe

3. Change it to the full path of your custom shell:

  Example:

  C:\BatchOS\SYSTEM\BOOT.exe



⚠️ WARNING: If BOOT.exe closes unexpectedly, Windows will log you out immediately.



-----------------------------------------------------

STEP 4: Reboot

-----------------------------------------------------

After reboot, your system will launch BOOT.exe instead of Explorer.



-----------------------------------------------------

STEP 5: Restore Explorer (Emergency)

-----------------------------------------------------

If AT-CMD exits or you want to go back to normal Windows:



1. Option 1: From AT-CMD MAIN_MENU, press '+' to restore Explorer.

2. Option 2: Press Ctrl+Alt+Del → Task Manager → File → Run new task → explorer.exe

3. Option 3: Boot into Safe Mode and set the Shell value back to:

  explorer.exe



-----------------------------------------------------

ADDITIONAL NOTES

-----------------------------------------------------

- Keep Explorer available as a backup.

- Make sure BOOT.exe is stable.

- You can always create a shortcut to explorer.exe on your AT-CMD menu for quick recovery.

