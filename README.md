Discord Wrapper for Portable Apps
===================


Currently, there isn't a great way to run Discord as a portable package.  It leaves data on the host system and isn't great at storing it's data somewhere other than the default location.  This wrapper allows the Discord to be dropped in unaltered and run as a Portable App on the [PortableApps.com](http://portableapps.com/) Platform.



Instructions
-------------
After downloading the contents of this repository, your directory structure should look like this:

```
+-- DiscordPortable
    +-- App
    |   +-- AppInfo
    |   |   +-- Launcher
    |   +-- Discord
    |   +-- DefaultData
    +-- Data
    +-- Other
        +-- Help
        |   +-- Images
        +-- Source
```

Download the [Discord Installer for Windows](https://discordapp.com/download) and extract the contents to a temporary directory and find a "nupkg" file.  Extract the contents of that file into a new directory.  Move the contents of the __lib\net45__ folder into __DiscordPortable\App\Discord__.

More information on creating PortableApps for the PortableApps.com platform can be found on the  [PortableApps.com Development Page](http://portableapps.com/development).

Known Issues
-------------
AppData folder must be copied to local drive on app startup and copied back to portable directory on app shut down.