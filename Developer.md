<img align="right" width="400" src="E-MU_0404_USB.jpg"/>

Building from source code
===================

1. Open the project in Xcode (double click src/EMUUSBAudio.xcodeproj)
2. Select Product/Build menu item
3. Select View/Navigators/Project Navigator menu item
4. right click on the  EMUUSBAudio.kext and click "Show in finder"
5. Copy the kext into the directory where the kextInstall script is

After that the kExtInstall script is ready for use (see Installation)





Tech notes
==========
The current version compiles with Xcode 5.1.1.
Original comes from source forge revision 7. http://sourceforge.net/projects/zaudiodrivermac/
But it did not compile on OSX 10.9 Mavericks. So I dumped part of the code, cleaned up, documented, 
refactored and wrote new code to get it working.

The present version is in a pretty bad shape. I did a major effort to refactor the input side of the code,
it's on the way but not yet polished. The rest of the code is still in original state.
Audio input and output (record and playback) are now working fine.
There are a few small loose ends and I'd like to clean up the code further.