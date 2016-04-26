MeshSceneScriptAccess
======================================

For example: `mesh_scene = BrainVoyager.ActiveDocument.MeshScene`.


### AddCurvatureFileForGroupCBA ###

```
x = mesh_scene.AddCurvatureFileForGroupCBA(a)
```

a : str
:	the curvature SMP file name

x : bool
:	success (`True` or `False`)


### AddMesh ###

```
x = mesh_scene.AddMesh(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### ClearGroupCBACurvatureFiles ###

```
mesh_scene.ClearGroupCBACurvatureFiles()
```


### Count ###

This is an int.


### CreateAverageCurvatureGroupMap ###

```
x = mesh_scene.CreateAverageCurvatureGroupMap()
```

x : bool
:	success (`True` or `False`)


### CreateAverageFoldedGroupMesh ###

```
x = mesh_scene.CreateAverageFoldedGroupMesh()
```

x : bool
:	success (`True` or `False`)


### CreateStandardSphereMesh ###

```
x = mesh_scene.CreateStandardSphereMesh()
```

x : str
:	the full path file SRF name


### CurrentMesh ###

This is a [MeshScriptAccess](./script_access.html#meshscriptaccess).


### Item ###

```
x = mesh_scene.Item(a)
```

a : int
:	the index

x : [MeshSceneScriptAccess](./script_access.html#meshscenescriptaccess)
:	the item


### LoadMesh ###

```
x = mesh_scene.LoadMesh(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### MapSphereMeshFromStandardSphere ###

```
x = mesh_scene.MapSphereMeshFromStandardSphere()
```

x : str
:	the full path SSM file name


### MergeMeshesInScene ###

```
x = mesh_scene.MergeMeshesInScene()
```

x : str
:	the full path SRF file name


### RunCBA ###

```
x = mesh_scene.RunCBA()
```

x : bool
:	success (`True` or `False`)


### RunRigidCBA ###

```
x = mesh_scene.RunRigidCBA(a)
```

a : str
:	the target PMP file name

x : bool
:	success (`True` or `False`)


### SaveSnapshotOfSurfaceWindow ###

```
x = mesh_scene.SaveSnapshotOfSurfaceWindow()
```

x : bool
:	success (`True` or `False`)


### SetStandardSphereToFoldedMesh ###

```
x = mesh_scene.SetStandardSphereToFoldedMesh(a)
```

a : str
:	the folded mesh file name

x : str
:	the full path SRF file name


### SphereResolutionCBA ###

This is an int.


### UpdateSurfaceWindow ###

```
mesh_scene.UpdateSurfaceWindow(a)
```

a : bool (optional)
:	process events (`True` or `False`)


### ViewpointPositionX ###

This is a float.


### ViewpointPositionY ###

This is a float.


### ViewpointPositionZ ###

This is a float.


### ViewpointRotationY ###

This is a float.


### ViewpointRotationX ###

This is a float.


### ViewpointRotationZ ###

This is a float.


### blockSignals ###

```
x = mesh_scene.blockSignals(a)
```

a : bool
:	`True` or `False`

x : bool
:	state before change (`True` or `False`)


### childEvent ###

```
mesh_scene.childEvent(a, b)
```

a : QChildEvent
:	?

b : ?
:	?


### children ###

```
x = mesh_scene.children()
```

x : tuple
:	?


### className ###

```
x = mesh_scene.className()
```

x : str
:	`'MeshSceneScriptAccess'`


### connect ###

```
x = mesh_scene.connect(a, b, c, d, e)
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
mesh_scene.customEvent(a, b)
```

a : QEvent
:	?

b : ?
:	?


### delete ###

```
mesh_scene.delete()
```


### deleteLater ###

```
mesh_scene.deleteLater()
```


### destroyed ###

```
mesh_scene.distroyed()
```


### disconnect ###

```
x = mesh_scene.disconnect(a, b, c, d)
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
mesh_scene.dumpObjectInfo(a)
```

a : ?
:	?


### dumpObjectTree ###

```
mesh_scene.dumpObjectTree(a)
```

a : ?
:	?

 
### dynamicPropertyNames ###

```
mesh_scene.dynamicPropertyNames(a)
```

a : ?
:	?

 
### event ###

```
x = mesh_scene.event(a)
```

a : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### eventFilter ###

```
x = mesh_scene.eventFilter(a, b)
```

a : QObject (?)
:	?

b : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### findChild ###

```
x = mesh_scene.findChild(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : QObject (?)
:	the child


### findChildren ###

```
x = mesh_scene.findChildren(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : tuple
:	the children


### help ###

```
mesh_scene.help()
```


### inherits ###

```
mesh_scene.inherits()
```


### installEventFilter ###

```
mesh_scene.installEventFilter(a)
```

a : QObject (?)
:	?


### isSignalConnected ###

```
x = mesh_scene.isSignalConnected(a)
```

a : QMethodSignal (?)
:	the signal

x : bool
:	`True` or `False`


### isWidgetType ###

```
x = mesh_scene.isWidgetType()
```

x : bool
:	`True` or `False`


### isWindowType ###

```
x = mesh_scene.isWindowType()
```

x : bool
:	`True` or `False`


### killTimer ###

```
mesh_scene.killTimer(a)
```

a : int
:	the id


### metaObject ###

```
x = mesh_scene.metaObject()
```

x : PythonQt.QtCore.QMetaObject (?)
:	?


### moveToThread ###

```
mesh_scene.moveToThread(a)
```

a : QThread
:	the thread


### objectName ###

This is a str.


### objectNameChanged ###

```
mesh_scene.objectNameChanged(a)
```

a : str (?)
:	?


### parent ###

```
x = mesh_scene.parent()
```

x : QObject (?)
:	?


### property ###

```
x = mesh_scene.property(a)
```

a : str (?)
:	the name

x : ?
:	?


### removeEventFilter ###

```
mesh_scene.removeEventFilter(a)
```

a : QObject (?)
:	?


### sender ###

```
mesh_scene.sender()
```

x : QObject (?)
:	?


### senderSignalIndex ###

```
mesh_scene.senderSignalIndex()
```

x : int
:	the index


### setObjectName ###

```
mesh_scene.setObjectName(a)
```

a : str
:	the name


### setParent ###

```
mesh_scene.setParent(a)
```

a : QObject
:	the parent


### setProperty ###

```
mesh_scene.setProperty(a)
```

a : str (?)
:	the property name

b : ?
:	the property value


### signalsBlocked ###

```
x = mesh_scene.signalsBlocked()
```

x : bool
:	`True` or `False`


### startTimer ###

```
x = mesh_scene.startTimer(a)
```

a : int
:	the interval

b : QT::TimeType (?)
:	the timer type (?)

x : int
:	?


### thread ###

```
mesh_scene.thread()
```


### timerEvent ###

```
mesh_scene.timerEvent(a)
```

a : QTimerEvent (?)
:	?


### tr ###

```
x = mesh_scene.tr(a, b, c)
```

a : QByteArray (?)
:	?

b : QByteArray (?)
:	?

c : int
:	?

x : str
:	?
