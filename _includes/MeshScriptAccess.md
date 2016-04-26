MeshScriptAccess
=================================

For example, `mesh = BrainVoyager.ActiveDocument.CurrentMesh`.


### AddStudyAndDesignMatrixAndCortexMapping ###

```
mesh.AddStudyAndDesignMatrixAndCortexMapping(a, b, c)
```

a : str
:	the functional file name

b : str
:	the design matrix file name

c : str
:	the SSM file name


### CalculateCurvature ###

```
mesh.CalculateCurvature()
```


### CalculateCurvatureCBA ###

```
mesh.CalculateCurvatureCBA()
```


### ClearDesignMatrix ###

```
mesh.ClearDesignMatrix()
```


### ClearMultiStudyGLMDefinition ###

```
mesh.ClearMultiStudyGLMDefinition()
```


### ComputeMultiStudyGLM ###

```
mesh.ComputeMultiStudyGLM()
```


### ComputeRFXGLM ###

```
mesh.ComputeRFXGLM()
```


### ComputeSingleStudyGLM ###

```
mesh.ComputeSingleStudyGLM()
```


### CorrectForSerialCorrelations ###

This is an int.


### CorrectInflatedSphereMesh ###

```
x = mesh.CorrectInflatedSphereMesh(a)
```

a : int
:	the number of cycles

x : bool
:	success (`True` or `False`)


### CreateMTCFromVTC ###

```
x = mesh.CreateMTCFromVTC(a, b, c)
```

a : float
:	the starting normal position

b : float
:	the ending normal position

c : str
:	the resulting MTC file name

x : bool
:	success (`True` or `False`)


### CreateMultiScaleCurvatureMap ###

```
x = mesh.CreateMultiScaleCurvatureMap(a, b, c, d)
```

a : int
:	the first smoothing level

b : int
:	the second smooting level

c : int
:	the third smoothing level

d : int
:	the fourth smoothing level

x : str
:	the file name (?)


### CreateSphericalCoordinatesMapFromSMP ###

```
x = mesh.CreateSphericalCoordinatesMapFromSMP(a)
```

a : str
:	the SMP on sphere file name

x : str
:	the file name (?)


### FileName ###

This is a str.


### FileNameOfPreprocessdMTC ###

This is a str.


### GetNameOfSurfaceMap ###

```
x = mesh.GetNameOfSurfaceMap(a)
```

a : int
:	the index

x : str
:	the name


### InflateMesh ###

```
x = mesh.InflateMesh(a, b, c)
```

a : int
:	the number of cycles

b : float
:	the smoothing force

c : str
:	the area reference mesh

x : bool
:	success (`True` or `False`)


### InflateMeshToSphere ###

```
x = mesh.InflateMeshToSphere(a)
```

a : int
:	the number of cycles

x : bool
:	success (`True` or `False`)


### LinearTrendRemoval ###

```
x = mesh.LinearTrendRemoval()
```

x : bool
:	success (`True` or `False`)


### LinkMTC ###

```
x = mesh.LinkMTC(a)
```

a : str
:	the MTC file name

x : bool
:	success (`True` or `False`)


### LoadGLM ###

```
x = mesh.LoadGLM(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### LoadMultiStudyGLMDefinitionFile ###

```
x = mesh.LoadMultiStudyGLMDefinitionFile(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### LoadSingleStudyGLMDesignMatrix ###

```
x = mesh.LoadSingleStudyGLMDesignMatrix(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### LoadSurfaceMaps ###

```
x = mesh.LoadSurfaceMaps(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### MeshScene ###

This is a [MeshSceneScriptAccess](./script_access.html#meshscenescriptaccess)


### MorphingUpdateInterval ###

This is an int.


### NrOfMTCVolumes ###

This is an int.


### NrOfSurfaceMaps ###

This is an int.


### NrOfVertices ###

This is an int.


### Save ###

```
mesh.Save()
```


### SaveAs ###

```
mesh.SaveAs(a)
```

a : str
:	the file name


### SaveGLM ###

```
mesh.SaveGLM(a)
```

a : str
:	the file name


### SaveMTC ###

```
mesh.SaveMTC(a)
```

a : str
:	the file name


### SaveMultiStudyGLMDefinitionFile ###

```
mesh.SaveMultiStudyGLMDefinitionFile(a)
```

a : str
:	the file name


### SaveSingleStudyGLMDesignMatrix ###

```
mesh.SaveSingleStudyGLMDesignMatrix(a)
```

a : str
:	the file name


### SaveSurfaceMaps ###

```
mesh.SaveSurfaceMaps(a)
```

a : str
:	the file name


### ShowGLM ###

```
mesh.ShowGLM()
```


### ShowSurfaceMap ###

```
mesh.ShowSurfaceMap(a)
```

a : int
:	the index


### SimplifyMesh ###

```
x = mesh.SimplifyMesh(a)
```

a : int
:	the number of target vertices

x : str
:	the file name (?)


### SmoothCurrentMap ###

```
mesh.SmoothCurrentMap(a)
```

a : int
:	the number of cycles


### SmoothMesh ###

```
x = mesh.SmoothMesh(a, b)
```

a : int
:	the number of cycles

b : float
:	the smoothing force

x : bool
:	success (`True` or `False`)


### SmoothRecoMesh ###

```
x = mesh.SmoothRecoMesh(a, b)
```

a : int
:	the number of cycles

b : float
:	the smoothing force

x : bool
:	success (`True` or `False`)


### SpatialSmoothing ###

```
x = mesh.SpatialSmoothing(a)
```

a : int
:	the number of cycles

x : bool
:	success (`True` or `False`)


### TemporalGaussianSmoothing ###

```
x = mesh.TemporalGaussianSmoothing(a, b)
```

a : float
:	the FWHM value

b : str
:	the unit of the FWHM value ("mm" or "px")

x : bool
:	success (`True` or `False`)


### TemporalHighPassFilterFFT ###

```
x = mesh.TemporalHighPassFilterFFT(a)
```

a : int
:	the number of cycles in time course

x : bool
:	success (`True` or `False`)


### UpdateAppearance ###

```
mesh.UpdateAppearance(a)
```

a : bool
:	process events (`True` or `False`)


### blockSignals ###

```
x = mesh.blockSignals(a)
```

a : bool
:	`True` or `False`

x : bool
:	state before change (`True` or `False`)


### childEvent ###

```
mesh.childEvent(a, b)
```

a : QChildEvent
:	?

b : ?
:	?


### children ###

```
x = mesh.children()
```

x : tuple
:	?


### className ###

```
x = mesh.className()
```

x : str
:	`'MeshScriptAccess'`


### connect ###

```
x = mesh.connect(a, b, c, d, e)
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
mesh.customEvent(a, b)
```

a : QEvent
:	?

b : ?
:	?


### delete ###

```
mesh.delete()
```


### deleteLater ###

```
mesh.deleteLater()
```


### destroyed ###

```
mesh.distroyed()
```


### disconnect ###

```
x = mesh.disconnect(a, b, c, d)
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
mesh.dumpObjectInfo(a)
```

a : ?
:	?


### dumpObjectTree ###

```
mesh.dumpObjectTree(a)
```

a : ?
:	?

 
### dynamicPropertyNames ###

```
mesh.dynamicPropertyNames(a)
```

a : ?
:	?

 
### event ###

```
x = mesh.event(a)
```

a : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### eventFilter ###

```
x = mesh.eventFilter(a, b)
```

a : QObject (?)
:	?

b : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### findChild ###

```
x = mesh.findChild(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : QObject (?)
:	the child


### findChildren ###

```
x = mesh.findChildren(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : tuple
:	the children


### help ###

```
mesh.help()
```


### inherits ###

```
mesh.inherits()
```


### installEventFilter ###

```
mesh.installEventFilter(a)
```

a : QObject (?)
:	?


### isSignalConnected ###

```
x = mesh.isSignalConnected(a)
```

a : QMethodSignal (?)
:	the signal

x : bool
:	`True` or `False`


### isWidgetType ###

```
x = mesh.isWidgetType()
```

x : bool
:	`True` or `False`


### isWindowType ###

```
x = mesh.isWindowType()
```

x : bool
:	`True` or `False`


### killTimer ###

```
mesh.killTimer(a)
```

a : int
:	the id


### metaObject ###

```
x = mesh.metaObject()
```

x : PythonQt.QtCore.QMetaObject (?)
:	?


### moveToThread ###

```
mesh.moveToThread(a)
```

a : QThread
:	the thread


### objectName ###

This is a str.


### objectNameChanged ###

```
mesh.objectNameChanged(a)
```

a : str (?)
:	?


### parent ###

```
x = mesh.parent()
```

x : QObject (?)
:	?


### property ###

```
x = mesh.property(a)
```

a : str (?)
:	the name

x : ?
:	?


### removeEventFilter ###

```
mesh.removeEventFilter(a)
```

a : QObject (?)
:	?


### sender ###

```
mesh.sender()
```

x : QObject (?)
:	?


### senderSignalIndex ###

```
mesh.senderSignalIndex()
```

x : int
:	the index


### setObjectName ###

```
mesh.setObjectName(a)
```

a : str
:	the name


### setParent ###

```
mesh.setParent(a)
```

a : QObject
:	the parent


### setProperty ###

```
mesh.setProperty(a)
```

a : str (?)
:	the property name

b : ?
:	the property value


### signalsBlocked ###

```
x = mesh.signalsBlocked()
```

x : bool
:	`True` or `False`


### startTimer ###

```
x = mesh.startTimer(a)
```

a : int
:	the interval

b : QT::TimeType (?)
:	the timer type (?)

x : int
:	?


### thread ###

```
mesh.thread()
```


### timerEvent ###

```
mesh.timerEvent(a)
```

a : QTimerEvent (?)
:	?


### tr ###

```
x = mesh.tr(a, b, c)
```

a : QByteArray (?)
:	?

b : QByteArray (?)
:	?

c : int
:	?

x : str
:	?
