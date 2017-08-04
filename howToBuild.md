How to build TrickEmu
==================================

Below are several methods and platforms for installing:

## Building on Unix-like systems via xbuild
1. Install Mono via your method of choice. (xbuild must be usable from your PATH)
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

## Building on Unix-like systems via MonoDevelop
1. Install MonoDevelop via your package manager. (dependencies already included)
2. Open a terminal within the TrickEmu folder or `cd` to it.
3. Run the `unix/unix_vs2md.sh` file from there. (usage info available in file)
4. Open `TrickEmu.sln` in MonoDevelop.
5. Change compile target from Debug to Release, if not already so.
6. Hit the compile button and you're done.

## Building on macOS via Xamarin Studio
1. DL/Install Xamarin Studio and dependencies from the [MonoDevelop site](monodevelop.com).
2. Edit `unix/unix_vs2md.sh` file to use macOS command instead of the GNU one.
3. Open a terminal within the TrickEmu folder or `cd` to it.
4. Run the `unix/unix_vs2md.sh` file from there.
5. Open `TrickEmu.sln` in Xamarin.
6. Change compile target from Debug to Release, if not already so.
7. Hit the compile button and you're done. 

## Building on Windows
1. Install Visual Studio 2015 (or 2012/2013) or SharpDevelop.
2. Open `TrickEmu.sln`.
3. Run a NuGet package restore.
4. Compile the project.


