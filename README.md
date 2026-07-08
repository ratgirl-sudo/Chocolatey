# Chocolatey
Chocolatey is a package manager for windows, but can be quite confusing to install if youre not very familiar with using powershell. I'm making this repo to try and help anyone having issues with the installation of it.

# Installation
Open powershell as an admiministrator (VERY important as it will not work when not in admin shell). Then, before running the installation command you need to check that the shell is not restricted by running Get-ExecutionPolicy.
Run Get-ExecutionPolicy , if after running the command you see Restricted as the response, you need to then run Set-ExecutionPolicy AllSigned . 
Now the shell is ready and unrestricted, the install command found below can be ran.
- Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
If no errors are displayed, you have done everything correctly! (good job!), you can now type choco into the powershell.
