# deralock
The DeraLock AntiVirus Trojan/Rogue from 2009. 
Has both NT 5.x (2k/XP/2003/XP x64/2003 x64) and NT 6.x (Vista/2008/Vista x64/2008 x64).
Windows 7, 2008 R2 and higher untested.

What it does:
Does a fake scan on the entire root drive (does cmd /a /s /w /q) (on Vista/2008, scans only Windows, System32 and Wbem folders),
Copies 4 files to your root drive (reg.exe, regedit.exe, taskkill.exe, shutdown.exe),
Kills Windows Explorer and Sidebar (Vista only),
If Windows XP Recovery Console is detected, it will delete its files,
Deletes HKLM, HKCU, HKU, HKCR and HKCC,
Deletes files from DllCache (Windows XP/2003 only),
runs attrib to remove system, hidden and read only attributes (the root drive and cmdcons (Recovery Console for XP/2003),
renames everything in Windows, System32, and Wbem folders to *.iaminyourpc,
Deletes all files with the extenstion, iaminyourpc,
Renames boot.1 to boot.ini (2K/XP/2003 only),
Restarts the computer.

WARNING: YOU SHOULD NOT RUN THIS TROJAN ON YOUR ACTUAL COMPUTER!! THIS WILL DESTROY ALL FOLDERS INCLUDING SYSTEM32, WINDOWS AND WBEM FOLDERS!
PLEASE, FOR YOUR SAFETY, USE A VIRTUAL MACHINE. I AM NOT RESPONSIBLE FOR ANY DAMAGE THAT IS DONE WHEN YOU RUN THIS ON YOUR ACTUAL COMPUTER!
BACK UP ANY DATA BEFORE YOU CONTINUE!

VirusTotal scans:
2000/XP/2003/XP x64/2003 x64: https://www.virustotal.com/gui/file/14295517acf7696525dd367a10fa4c9ba7454d6f35b35465f6b83dd82eb6cc6e/details
Vista/2008/Vista x64/2008 x64: https://www.virustotal.com/gui/file/ceeff2242cb1f2741cdbfaac8f7059b0759225e579f3f8ee3d15f7b332e37a10/detection
