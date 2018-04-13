# CarrotBinaries Mac Download Instructions

1) Download and copy carrot.dmg to desired folder 

2) Double click the carrot.dmg

3) Drag Carrot Core icon to the Applications 

4) Launch Carrot Core

Note: On Carrot Core launch if you get this error

```
Dyld Error Message:
  Library not loaded: @loader_path/libboost_system-mt.dylib
  Referenced from: /Applications/Carrot-Qt.app/Contents/Frameworks/libboost_thread-mt.dylib
  Reason: image not found
```
You will need to copy libboost_system.dylib to libboost_system-mt.dylib in the /Applications/Carrot-Qt.app/Contents/Frameworks folder  
  