How to build TrickEmu
==================================

Below are several methods and platforms for installing:

##Building on Unix-like systems via xbuild
1. Install Mono via your method of choice. (make sure you can use xbuild from your PATH.
2. Open a terminal window.
3. Change directory to the TrickEmu folder
4. Restore Nuget packages with: 
```
nuget restore TrickEmu.sln
```
5. Enter the command below:
```
xbuild /p:Configuration=Release /p:TargetFrameworkVersion=v4.5 TrickEmu.sln
```

##Building on Unix-like systems via MonoDevelop
1. Install MonoDevelop via your package manager. (dependencies already included)
2. Run the unix/unix_vs2md.sh file from. (usage info is inside bash file)
3. Open TrickEmu.sln in MonoDevelop.
4. Change compile target from Debug to Release, if not already so.
5. Hit the compile button and you're done.

##Building on macOS via Xamarin Studio
1. DL/Install Xamarin Studio and dependencies from the [MonoDevelop site](monodevelop.com).
2. Edit the unix/unix_vs2md.sh file to use macOS command instead of the GNU one.
3. Run unix/unix_vs2md.sh file from the TrickEmu folder in a terminal.
4. Open TrickEmu.sln in Xamarin.
5. Change compile target from Debug to Release, if not already so.
6. Hit the compile button and you're done. 

##Building on Windows
1. Install Visual Studio 2015 (or 2012/2013) or SharpDevelop.
2. Open TrickEmu.sln.
3. Run a NuGet package restore.
4. Compile the project.


