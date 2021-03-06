GAMADV-X
========
GAMADV-X is a free, open source command line tool for Google G Suite Administrators to manage domain and user settings quickly and easily.

GAMADV-X is a rewrite/extension of Jay Lee's [GAM](https://github.com/jay0lee/GAM), without his efforts, this version wouldn't exist.

Documentation
-------------
General GAM documentation is hosted in the [GitHub Wiki]. Documentation specifically for GAMADV-X is in Gam*.txt files.

Downloads
---------
You can download the current GAMADV-X release from the [GitHub Releases] page. Choose one of the following:

* Single Executable, Linux/Mac OS - `gamadv-x-4.wx.yz-linux-x86_64.xz, gamadv-x-4.wx.yz-macos.tar.xz`
  - Download the archive, extract the contents into some directory.
  - Start a terminal session and cd to the install directory.

* Single Executable Archive, Windows - `gamadv-x-x.yy.z-windows-x64.zip, gamadv-x-4.wx.yz-windows.zip`
  - Download the archive, extract the contents into some directory.
  - Start a terminal session and cd to the install directory.

* Single Executable Installer, Windows - `gamadv-x-4.wx.yz-windows-x64.msi`
  - Download the installer and run it.
  - Start a Command Prompt/PowerShell session and cd to the install directory.

* Source, all platforms - Source code(zip), Source code(tar.gz)
  - Download the archive, extract the contents into some directory.
  - Start a terminal/Command Prompt/PowerShell session and cd to the install directory.

Installation - New Users
------------------------
Read GamConfig.txt.

Enter the following gam commands and follow instructions to create the necessary authorizations.
- Build gam.cfg: ```gam config verify```
- Build GAM Project for authorization: ```gam create project```
- Authorize Gam Client: ```gam oauth create```
- Authorize Service Account: ```gam user <admin email address> check serviceaccount```

Installation - Upgrading from a GAM version other than a prior version of GAMADV-X
----------------------------------------------------------------------------------
Read GamConfig.txt.

Set the environment variable OLDGAMPATH to the location of your existing client_secrets.json/oauth2service.json files;
they will be copied to a new location. The prior versions remain where they were so that both your old and this new
version of GAM can run. Your existing oauth2.txt is not used, a new file will be built for this version of GAM.

Enter the following gam commands and follow instructions.
- Build gam.cfg: ```gam config verify```
- Authorize Gam Client: ```gam oauth create```
- Authorize Service Account: ```gam user <admin email address> check serviceaccount```

Installation - Upgrading from a prior version of GAMADV-X
---------------------------------------------------------
Read GamUpdate.txt

Mailing List / Discussion group
-------------------------------
The GAM mailing list / discussion group is hosted on [Google Groups].  You can join the list and interact via email, or just post from the web itself.

Source Repository
-----------------
The official GAMADV-X source repository is on [GitHub] in the master branch.

Author
------
GAMADV-X is maintained by <a href="mailto:ross.scroggs@gmail.com">Ross Scroggs</a>.

[GitHub Releases]: https://github.com/taers232c/GAMADV-X/releases
[GitHub]: https://github.com/taers232c/GAMADV-X/tree/master
[GitHub Wiki]: https://github.com/taers232c/GAMADV-X/wiki/
[Google Groups]: http://groups.google.com/group/google-apps-manager
