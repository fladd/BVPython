BrainVoyagerScriptAccess
=========================================

The readily available object `BrainVoyager` is an instance of this class.


### ActiveDocument ###

This is a [DocumentScriptAccess](./scrip_access.html#documentscriptaccess).


### BrowseDirectory ###

```
x = BrainVoyager.BrowseDirectory(a)
```

a : str
:	the path (e.g. `"./Desktop"`)

x : str
:	the selected directory


### BrowseFile ###

```
x = BrainVoyager.BrowseFile(a, b)
```

a : str
:	the path (e.g. `"./Desktop/"`)

b : str
:	a filemask (e.g. `"*.txt"`)

x : str
:	the selcted file


### BuildNumber ###

This is an int.


### CallPluginFunction ###

```
x = BrainVoyager.CallPluginFunction(a)
```

a : str (?)
:	the path (e.g. `"./Desktop/"`)

x : bool
:	success (`True` or `False`)


### CreateProjectAMR ###

```
x = BrainVoyager.CreateProjectAMR(a, b, c, d, e, f, g)
```

a : str
:	the filetype (`"DICOM"`, `"SIEMENS"`, `"GE_I"` (no parameters for +20 logic like in GUI), `"GE_MR"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : bool
:	swap byte order (`True` or `False`)

e : int
:	the size of the image along x-axis

f : int
:	the size of the image along y-axis

g : int
:	the number of bytes per pixel

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document


### CreateProjectDMR ###

```
x = BrainVoyager.CreateProjectDMR(a, b, c, d, e, f, g, h, i, j, k, l)
```

a : str
:	the filetype (`"DICOM"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : int
:	the number of volumes to skip

e : bool
:	create AMR (`True` or `False`)

f : int
:	the number of slices in a volume

g : str
:	the STC prefix

h : bool
:	swap byte order (`True` or `False`)

i : int
:	the size of the image along x-axis

j : int
:	the size of the image along y-axis

k : int
:	the number of bytes per pixel

l : str
:	the directory to save to

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	The document


### CreateProjectFMR ###

```
x = BrainVoyager.CreateProjectFMR(a, b, c, d, e, f, g, h, i, j, k, l)
```

a : str
:	the filetype (`"DICOM"`, `"SIEMENS"`, `"GE_I"` (no parameters for +20 logic like in GUI), `"GE_MR"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : int
:	the number of volumes to skip

e : bool
:	create AMR (`True` or `False`)

f : int
:	the number of slices in a volume

g : str
:	the STC prefix

h : bool
:	swap byte order (`True` or `False`)

i : int
:	the size of the image along x-axis

j : int
:	the size of the image along y-axis

k : int
:	the number of bytes per pixel

l : str
:	the directory to save to

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	The document


### CreateProjectFMRSlicesTimeLooping ###

```
x = BrainVoyager.CreateProjectFMRSlicesTimeLooping(a, b, c, d, e, f, g, h, i, j, k, l)
```

a : str
:	the filetype (`"DICOM"`, `"SIEMENS"`, `"GE_I"` (no parameters for +20 logic like in GUI), `"GE_MR"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : int
:	the number of volumes to skip

e : bool
:	create AMR (`True` or `False`)

f : int
:	the number of slices in a volume

g : str
:	the STC prefix

h : bool
:	swap byte order (`True` or `False`)

i : int
:	the size of the image along x-axis

j : int
:	the size of the image along y-axis

k : int
:	the number of bytes per pixel

l : str
:	the directory to save to

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	The document


### CreateProjectMosaicDMR ###

```
x = BrainVoyager.CreateProjectMosaicDMR(a, b, c, d, e, f, g, h, i, j, k, l, m, n, o)
```

a : str
:	the filetype (`"DICOM"`, `"SIEMENS"`, `"GE_I"` (no parameters for +20 logic like in GUI), `"GE_MR"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : int
:	the number of volumes to skip

e : bool
:	create AMR (`True` or `False`)

f : int
:	the number of slices in a volume

g : str
:	the STC prefix

h : bool
:	swap byte order (`True` or `False`)

i : int
:	the mosaic size of images in volume along x-axis

j : int
:	the mosaic size of the images in volume along y-axis

k : int
:	the number of bytes per pixel

l : str
:	the directory to save to

m : int
:	the number of volumes per image

n : int
:	the dimension of image along x-axis

o : int
:	the dimension of image along y-axis

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document


### CreateProjectMosaicFMR ###

```
x = BrainVoyager.CreateProjectMosaicFMR(a, b, c, d, e, f, g, h, i, j, k, l, m, n, o)
```

a : str
:	the filetype (`"DICOM"`, `"SIEMENS"`, `"GE_I"` (no parameters for +20 logic like in GUI), `"GE_MR"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : int
:	the number of volumes to skip

e : bool
:	create AMR (`True` or `False`)

f : int
:	the number of slices in a volume

g : str
:	the STC prefix

h : bool
:	swap byte order (`True` or `False`)

i : int
:	the mosaic size of images in volume along x-axis

j : int
:	the mosaic size of the images in volume along y-axis

k : int
:	the number of bytes per pixel

l : str
:	the directory to save to

m : int
:	the number of volumes per image

n : int
:	the dimension of image along x-axis

o : int
:	the dimension of image along y-axis

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document


### CreateProjectVMR ###

```
x = BrainVoyager.CreateProjectVMR(a, b, c, d, e, f, g)
```

a : str
:	the filetype (`"DICOM"`, `"SIEMENS"`, `"GE_I"` (no parameters for +20 logic like in GUI), `"GE_MR"`, `"PHILIPS_REC"` or `"ANALYZE"`)

b : str
:	the full path to first file

c : int
:	the number of volumes

d : bool
:	swap byte order (`True` or `False`)

e : int
:	the size of the image along x-axis

f : int
:	the size of the image along y-axis

g : int
:	the number of bytes per pixel

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document


### CurrentDirectory ###

This is a str.


### Documents ###

This is a
[DocumentListScriptAccess](./script_access.html#documentlistscriptaccess).


### ExecutePlugin ###

```
x = BrainVoyager.ExecutePlugin()
```

x : bool
:	success (`True` or `False`)


### Exit ###

```
BrainVoyager.Exit()
```


### FindChild ###

```
x = BrainVoyager.FindChild(a)
```

a : str
:	the widget name

x : QObject
:	`QObject`


### GetPluginFloatParameter ###

```
x = BrainVoyager.GetPluginFloatParameter(a)
```

a : str
:	the parameter name

x : float
:	the parameter value


### GetPluginIntParameter ###

```
x = BrainVoyager.GetPluginIntParameter(a)
```

a : str
:	the parameter name

x : int
:	the paramter value


### GetPluginStringParameter ###

```
x = BrainVoyager.GetPluginStringParameter(a)
```

a : str
:	the parameter name

x : str
:	the parameter value

 
### GetVTCsOfMDM ###

```
x = BrainVoyager.GetVTCsOfMDM(a)
```

a : str
:	the MDM filename

x : tuple
:	the VTCs


### HideScriptsWindow ###

```
BrainVoyager.HideScriptsWindow()
```


### Is64Bits ###

This is a bool.


### MessageBox ###

```
BrainVoyager.MessageBox(a)
```

a : str
:	the message


### MoveWindow ###

```
BrainVoyager.MoveWindow(a, b)
```

a : int
:	the new x position

b : int
:	the new y position


### OpenDocument ###

```
x = BrainVoyager.OpenDocument(a)
```

a : int
:	the full path to file

x : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document


### PathToData ###

This is a str.


### PathToSampleData ###

This is a str.


### PrintToLog ###

```
BrainVoyager.PrintToLog(a)
```

a : str
:	the content to print


### RenameDicomFilesInDirectory ###

```
BrainVoyager.RenameDicomFilesInDirectory(a)
```

a : str
:	the new name


### ResizeWindow ###

```
BrainVoyager.ResizeWindow(a, b)
```

a : int
:	the new x size

b : int
:	the new y size


### SetPluginFloatParameter ###

```
BrainVoyager.SetPluginFloatParameter(a, b)
```

a : str
:	the parameter name

b : float
:	the paramter value


### SetPluginIntParameter ###

```
BrainVoyager.SetPluginIntParameter(a, b)
```

a : str
:	the parameter name

b : int
:	the paramter value


### SetPluginStringParameter ###

```
BrainVoyager.SetPluginStringParameter(a, b)
```

a : str
:	the parameter name

b : str
:	the paramter value


### ShowLogTab ###

```
BrainVoyager.ShowLogTab()
```


### ShowScriptsWindow ###

```
BrainVoyager.ShowScriptsWindow()
```


### TimeOutMessageBox ###

```
x = BrainVoyager.TimeOutMessageBox(a, b)
```

a : str
:	the message

b : int
:	the duration

x : bool
:	success (`True` or `False`)


### VersionMajor ###

This is an int.


### VersionMinor ###

This is an int.


### VersionPatch ###

This is an int.


### VOIFileName ###

This is a str.


### blockSignals ###

```
x = BrainVoyager.blockSignals(a)
```

a : bool
:	`True` or `False`

x : bool
:	state before change (`True` or `False`)


### childEvent ###

```
BrainVoyager.childEvent(a, b)
```

a : QChildEvent
:	?

b : ?
:	?


### children ###

```
x = BrainVoyager.children()
```

x : tuple
:	?


### className ###

```
x = BrainVoyager.className()
```

x : str
:	`'BrainVoyagerScriptAccess'`


### connect ###

```
x = BrainVoyager.connect(a, b, c, d, e)
```

a : QObject (?)
:	the sender

b : QByteArray (?)
:	the signal

c : QObject (?)
:	the receiver

d : QByteArray (?)
:	the slot

e : Qt::ConnectionType (?)
:	the connection type

x : bool
:	`True` or `False`


### customEvent ###

```
BrainVoyager.customEvent(a, b)
```

a : QEvent
:	?

b : ?
:	?


### delete ###

```
BrainVoyager.delete()
```


### deleteLater ###

```
BrainVoyager.deleteLater()
```


### destroyed ###

```
BrainVoyager.distroyed()
```


### disconnect ###

```
x = BrainVoyager.disconnect(a, b, c, d)
```

a : QObject (?)
:	the sender (?)

b : QByteArray (?)
:	the signal (?)

c : QObject (?)
:	the receiver (?)

d : QByteArray (?)
:	the slot (?)

x : bool
:	`True` or `False`


### dumpObjectInfo ###

```
BrainVoyager.dumpObjectInfo(a)
```

a : ?
:	?


### dumpObjectTree ###

```
BrainVoyager.dumpObjectTree(a)
```

a : ?
:	?

 
### dynamicPropertyNames ###

```
BrainVoyager.dynamicPropertyNames(a)
```

a : ?
:	?

 
### event ###

```
x = BrainVoyager.event(a)
```

a : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### eventFilter ###

```
x = BrainVoyager.eventFilter(a, b)
```

a : QObject (?)
:	?

b : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### findChild ###

```
x = BrainVoyager.findChild(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : QObject (?)
:	the child


### findChildren ###

```
x = BrainVoyager.findChildren(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : tuple
:	the children


### h ###

This is an int.


### help ###

```
BrainVoyager.help()
```


### inherits ###

```
BrainVoyager.inherits()
```


### installEventFilter ###

```
BrainVoyager.installEventFilter(a)
```

a : QObject (?)
:	?


### isSignalConnected ###

```
x = BrainVoyager.isSignalConnected(a)
```

a : QMethodSignal (?)
:	the signal

x : bool
:	`True` or `False`


### isWidgetType ###

```
x = BrainVoyager.isWidgetType()
```

x : bool
:	`True` or `False`


### isWindowType ###

```
x = BrainVoyager.isWindowType()
```

x : bool
:	`True` or `False`


### killTimer ###

```
BrainVoyager.killTimer(a)
```

a : int
:	the id


### metaObject ###

```
x = BrainVoyager.metaObject()
```

x : PythonQt.QtCore.QMetaObject (?)
:	?


### moveToThread ###

```
BrainVoyager.moveToThread(a)
```

a : QThread
:	the thread


### objectName ###

This is a str.


### objectNameChanged ###

```
BrainVoyager.objectNameChanged(a)
```

a : str (?)
:	?


### parent ###

```
x = BrainVoyager.parent()
```

x : QObject (?)
:	?


### property ###

```
x = BrainVoyager.property(a)
```

a : str (?)
:	the name

x : ?
:	?


### removeEventFilter ###

```
BrainVoyager.removeEventFilter(a)
```

a : QObject (?)
:	?


### sender ###

```
BrainVoyager.sender()
```

x : QObject (?)
:	?


### senderSignalIndex ###

```
BrainVoyager.senderSignalIndex()
```

x : int
:	the index


### setObjectName ###

```
BrainVoyager.setObjectName(a)
```

a : str
:	the name


### setParent ###

```
BrainVoyager.setParent(a)
```

a : QObject
:	the parent


### setProperty ###

```
BrainVoyager.setProperty(a)
```

a : str (?)
:	the property name

b : ?
:	the property value


### signalsBlocked ###

```
x = BrainVoyager.signalsBlocked()
```

x : bool
:	`True` or `False`


### startTimer ###

```
x = BrainVoyager.startTimer(a)
```

a : int
:	the interval

b : QT::TimeType (?)
:	the timer type (?)

x : int
:	?


### thread ###

```
BrainVoyager.thread()
```


### timerEvent ###

```
BrainVoyager.timerEvent(a)
```

a : QTimerEvent (?)
:	?


### tr ###

```
x = BrainVoyager.tr(a, b, c)
```

a : QByteArray (?)
:	?

b : QByteArray (?)
:	?

c : int
:	?

x : str
:	?


### value ###

This is an int.


### visible ###

This is a bool.


### w ###

This is an int.


### x ###

This is an int.


### y ###

This is an int.
