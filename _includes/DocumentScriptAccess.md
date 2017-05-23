DocumentScriptAccess
=====================================

Opened AMR, DMR, FMR and VMR documents are instances of this class.
For example: `document = BrainVoyager.ActiveDocument`.


### AddCondition ###

```
document.AddCondition(a)
```

a : str
:	the condition name


### AddContrast ###

```
document.AddContrast(a)
```

a : str
:	the contrast name


### AddInterval ###

```
document.AddInterval(a, b, c)
```

a : str
:	the condition name

b : int
:	lower bound

c : int
:	upper bound


### AddMesh ###

```
x = document.AddMesh(a)
```

a : str
:	the mesh file name

x : bool
:	success (`True` or `False`)


### AddPredictor ###

```
document.AddPredictor(a)
```

a : str
:	the predictor name


### AddROIContrast ###

```
document.AddROIContrast(a)
```

a : str
:	the contrast name

b : str
:	the contrast content


### AddStudyAndDesignMatrix ###

```
document.AddStudyAndDesignMatrix(a, b)
```

a : str
:	the functional file name

b : str
:	the design matrix file name


### AdjustMeanIntensity ###

```
x = document.AdjustMeanIntensity()
```

x : bool
:	success (`True` or `False`)


### ApplyHemodynamicResponseFunctionToPredictor ###

```
document.ApplyHemodynamicResponseFunctionToPredictor(a)
```

a : str
:	the predictor name


### AutoACPCAndTALTransformation ###

```
x = document.AutoACPCAndTALTransformation()
```

x : bool
:	success (`True` or `False`)


### AutoTransformToIsoVoxel ###

```
x = document.AutoTransformToIsoVoxel(a, b)
```

a : int
:	the interpolation value

b : str
:	the ISO VMR file name

x : bool
:	success (`True` or `False`)


### AutoTransformToSAG ###

```
x = document.AutoTransformToSAG(a)
```

a : str
:	the saggital VMR file name

x : bool
:	success (`True` or `False`)


### ClearContrasts ###

```
document.ClearContrasts()
```


### ClearDesignMatrix ###

```
document.ClearDesignMatrix()
```


### ClearMultiStudyGLMDefinition ###

```
document.ClearMultiStudyGLMDefinition()
```


### ClearStimulationProtocol ###

```
document.ClearStimulationProtocol()
```


### Close ###

```
document.Close()
```


### ComputeMultiStudyGLM ###

```
document.ComputeMultiStudyGLM()
```


### ComputeRFXGLM ###

```
document.ComputeRFXGLM()
```

### ComputeSingleStudyGLM ###

```
document.ComputeSingleStudyGLM()
```


### ComputeSingleStudyGLMForVOI ###

```
document.ComputeSingleStudyGLMForVOI()
```


### CoregisterFMRToVMR ###

```
x = document.CoregisterFMRToVMR(a, b)
```

a : str
:   the FMR file name

b : int
:   use original FMR volume (0) or AMR (1; recommended)

x : bool
:   success


### CoregisterFMRToVMRUsingBBR ###

```
x = document.CoregisterFMRToVMRUsingBBR(a)
```

a : str
:   the FMR file name

x : bool
:   success


### CorrectForSerialCorrelations ###

This is an int.


### CorrectIntensityInhomogeneities ###

```
x = document.CorrectIntensityInhomogeneities()
```

x : bool
:	success (`True` or `False`)


### CorrectMotion ###

```
x = document.CorrectMotion(a)
```

a : int
:	the target volume

x : bool
:	success (`True` or `False`)


### CorrectMotionEx ###

```
x = document.CorrectMotionEx(a, b, c, d, e, f)
```

a : int
:	the target volume

b : int
:	the interpolation method (0 and 1: trilinear detection and trilinear
    interpolation, 2: trilinear detection and sinc interpolation or 3: sinc
    detection of motion and sinc interpolation)

c : bool
:	use full data set (`True` or `False`)

d : int
:	the maximum number of iterations

e : bool
:	generate movies (`True` or `False`)

f : bool
:	generate extended log file (`True` or `False`)

x : bool
:	success (`True` or `False`)


### CorrectMotionTargetVolumeInOtherRun ###

```
x = document.CorrectMotionTargetVolumeInOtherRun(a, b)
```

a : str
:	the target FMR file name

b : int
:	the target volume

x : bool
:	success (`True` or `False`)


### CorrectMotionTargetVolumeInOtherRunEx ###

```
x = document.CorrectMotionTargetVolumeInOtherRunEx(a, b, c, d, e, f, g)
```

a : str
:	the target FMR file name

b : int
:	the target volume

c : int
:	the interpolation method (0 and 1: trilinear detection and trilinear
    interpolation, 2: trilinear detection and sinc interpolation or 3: sinc
    detection of motion and sinc interpolation)

d : bool
:	use full data set (`True` or `False`)

e : int
:	the maximum number of iterations

f : bool
:	generate movies (`True` or `False`)

g : bool
:	generate extended log file (`True` or `False`)

x : bool
:	success (`True` or `False`)


### CorrectSliceTiming ###

```
x = document.CorrectSliceTiming(a, b)
```

a : str
:	the slice order (0: Ascending, 1: Ascending-interleaved,
    2: Ascending-interleaved 2 (Siemens only), 10: Descending,
    11: Descending-interleaved, 12: Descending-interleaved 2)

b : int
:	the interpolation method (0: trilinear, 1: cubic spline, 2: windowed SINC)

x : bool
:	success (`True` or `False`)


### CorrectSliceTimingUsingTimeTable ###

```
x = document.CorrectSliceTimingUsingTimeTable(a)
```

a : int
:	the interpolation method (0: trilinear, 1: cubic spline, 2: windowed SINC)

x : bool
:	success (`True` or `False`)


### CorrectSliceTimingWithSliceOrder ###

```
x = document.CorrectSliceTimingWithSliceOrder(a, b)
```

a : str
:	the slice number order (e.g. ""1 14 2 15 3 16")

b : int
:	the interpolation method (0: trilinear, 1: cubic spline, 2: windowed SINC)

x : bool
:	success (`True` or `False`)

  
### CreateMTCFromVTC ###

```
x = document.CreateMTCFromVTC(a, b, c)
```

a : float
:	the sampling depth inside white matter

b : float
:	the sampling depth inside grey matter

c : str
:	the resulting MTC file name

x : bool
:	success (`True` or `False`)


### CreateVDWInACPCSpace ###

```
x = document.CreateVDWInACPCSpace(a, b, c, d, e, f, g, h, i)
```

a : str
:	the DMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the ACPC file name

e : str
:	the resulting VDW file name

f : int
:	the data type (1: integer 2-byte format, 2: float format)

g : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

h : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

i : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)


### CreateVDWInTALSpace ###

```
x = document.CreateVDWInTALSpace(a, b, c, d, e, f, g, h, i, j)
```

a : str
:	the DMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the ACPC file name

e : str
:	the TAL file name

f : str
:	the resulting VDW file name

g : int
:	the data type (1: integer 2-byte format, 2: float format)

h : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

i : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

j : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)


### CreateVDWInVMRSpace ###

```
x = document.CreateVDWInVMRSpace(a, b, c, d, e, f, g, h)
```

a : str
:	the DMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the resulting VDW file name

e : int
:	the data type (1: integer 2-byte format, 2: float format)

f : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

g : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

h : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)


### CreateVTC ###

```
x = document.CreateVTC(a, b, c, d, e, f)
```

a : str
:	the FMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the ACPC file name

e : str
:	the TAL file name

f : str
:	the resulting VTC file name

x : bool
:	success (`True` or `False`)


### CreateVTCInACPCSpace ###

```
x = document.CreateVTCInACPCSpace(a, b, c, d, e, f, g, h, i)
```

a : str
:	the FMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the ACPC file name

e : str
:	the resulting VTC file name

f : int
:	the data type (1: integer 2-byte format, 2: float format)

g : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

h : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

i : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)


### CreateVTCInMNISpace ###

```
x = document.CreateVTCInMNISpace(a, b, c, d, e, f, g, h, i)
```

a : str
:	the FMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:   the TRF file name

e : str
:	the resulting VTC file name

f : int
:	the data type (1: integer 2-byte format, 2: float format)

g : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

h : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

i : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)

### CreateVTCInTALSpace ###

```
x = document.CreateVTCInTALSpace(a, b, c, d, e, f, g, h, i, j)
```

a : str
:	the FMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the ACPC file name

e : str
:	the TAL file name

f : str
:	the resulting VTC file name

g : int
:	the data type (1: integer 2-byte format, 2: float format)

h : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

i : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

j : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)


### CreateVTCInVMRSpace ###

```
x = document.CreateVTCInVMRSpace(a, b, c, d, e, f, g, h)
```

a : str
:	the FMR file name

b : str
:	the IA file name

c : str
:	the FA file name

d : str
:	the resulting VTC file name

e : int
:	the data type (1: integer 2-byte format, 2: float format)

f : int
:	the resolution (1, 2 or 3; e.g. 1: 1 x 1 x 1 mm)

g : int
:	the interpolation method (0: nearest neighbor, 1: trilinear, 2: sinc)

h : int
:	the bounding box intensity threshold (default = 100)

x : bool
:	success (`True` or `False`)


### CurrentMesh ###

This is a [MeshScriptAccess](./script_access.html#meshscriptaccess).


### DeselectVOI ###

```
document.DeselectVOI(a)
```

a : int
:	the VOI index


### DimX ###

This is an int.


### DimY ###

This is an int.


### DimX ###

This is an int.


### ExtendedTALSpaceForVTCCreation ###

This is a bool.


### FileName ###

This is a str.


### FileNameOfCurrentVTC ###

This is an str.


### FileNameOfPreprocessdFMR ###

This is a str.


### FirstConfoundPredictorOfSDM ###

This is an int.


### GapThickness ###

This is a float.


### GetBetaNameOfROIGLM ###

```
x = document.GetBetaNameOfROIGLM(a)
```

a : int
:	the beta index

x : str
:	the name


### GetBetaValueOfROIGLM ###

```
x = document.GetBetaValueOfROIGLM(a)
```

a : int
:	the beta index

x : float
:	the value


### GetFMRDataAsDoubleList ###

```
x = document.GetFMRDataAsDoubleList()
```

x : tuple
:	the FMR data as float values


### GetMeshScene ###

```
x = document.GetMeshScene()
```

x : [MeshSceneScriptAccess](./script_access.html#meshscenescriptaccess)
:	the mesh scene


### GetNameOfROIContrast ###

```
x = document.GetNameOfROIContrast(a)
```

a : int
:	the contrast index

x : str
:	the contrast name


### GetNameOfVOI ###

```
x = document.GetNameOfVOI(a)
```

a : int
:	the VOI index

x : str
:	the VOI name


### GetNameOfVolumeMap ###

```
x = document.GetNameOfVolumeMap(a)
```

a : int
:	the volume map index

x : str
:	the volume map name


### GetPValueOfROIContrast ###

```
x = document.GetPValueOfROIContrast(a)
```

a : int
:	the contrast index

x : float
:	the p-value


### GetTValueOfROIContrast ###

```
x = document.GetTValueOfROIContrast(a)
```

a : int
:	the contrast index

x : float
:	the t-value


### GetVolumeDataAsByteBuffer ###

```
x = document.GetVolumeDataAsByteBuffer()
```

x : PythonQt.QtCore.QByteArray
:	the byte buffer


### GetVolumeDataAsDoubleList ###

```
x = document.GetVolumeDataAsDoubleList()
```

x : tuple
:	the data as float values


### GetVolumeDataAsIntList ###

```
x = document.GetVolumeDataAsIntList()
```

x : tuple
:	the data as integer values


### GetVoxelIntensity ###

```
x = document.GetVoxelIntensity(a, b, c)
```

a : int
:	the x coordinate

b : int
:	the y coordinate

c : int
:	the z coordinate

x : int
:	the voxel intensity value


### HasSliceTimeTable ###

This is a bool.


### HideAllVOIs ###

```
document.HideAllVOIs()
```


### HideVolumeMapsDlg ###


```
document.HideVolumeMapsDlg()
```


### InterSliceTime ###

This is an int.


### LinearTrendRemoval ###

```
x = document.LinearTrendRemoval()
```

x : bool
:	success (`True` or `False`)


### LinkAMR ###

```
x = document.LinkAMR(a)
```

a : str
:	the AMR file name

x : bool
:	success (`True` or `False`)


### LinkMTC ###

```
x = document.LinkMTC(a)
```

a : str
:	the MTC file name

x : bool
:	success (`True` or `False`)


### LinkStimulationProtocol ###

```
x = document.LinkStimulationProtocol(a)
```

a : str
:	the protocol file name

x : bool
:	success (`True` or `False`)


### LinkVTC ###

```
x = document.LinkVTC(a)
```

a : str
:	the VTC file name

x : bool
:	success (`True` or `False`)


### LoadGLM ###

```
x = document.LoadGLM(a)
```

a : str
:	the GLM file name

x : bool
:	success (`True` or `False`)


### LoadMesh ###

```
x = document.LoadMesh(a)
```

a : str
:	the Mesh file name

x : bool
:	success (`True` or `False`)


### LoadMultiStudyGLMDefinitionFile ###

```
x = document.LoadMultiStudyGLMDefinitionFile(a)
```

a : str
:	the MDM file name

x : bool
:	success (`True` or `False`)


### LoadSingleStudyGLMDesignMatrix ###

```
x = document.LoadSingleStudyGLMDesignMatrix(a)
```

a : str
:	the SDM file name

x : bool
:	success (`True` or `False`)


### LoadVOIFile ###

```
x = document.LoadVOIFile(a)
```

a : str
:	the VOI file name

x : bool
:	success (`True` or `False`)


### LoadVolumeMaps ###

```
x = document.LoadVolumeMaps(a)
```

a : str
:	the volume maps file name

x : bool
:	success (`True` or `False`)


### MeshScene ###

This is a [MeshSceneScriptAccess](./script_access.html#meshscenescriptaccess).


### MotionCorrection3D ###

```
x = document.MotionCorrection3D()
```

x : bool
:	success (`True` or `False`)


### NormalizeToMNISpace ###

```
document.NormalizeToMNISpace()
```


### NrOfPredictorsInSingleStudyDM ###

This is an int.


### NrOfROIContrasts ###

This is an int.


### NrOfSkippedVolumes ###

This is an int.


### NrOfSlices ###

This is an int.


### NrOfTimePointsInSingleStudyDM ###

This is an int.


### NrOfVOIs ###

This is an int.


### NrOfVolumeMaps ###

This is an int.


### NrOfVolumes ###

This is an int.


### PSCTransformStudies ###

This is a bool.


### PathFileName ###

This is a str.


### PixelSizeOfSliceDimX ###

This is a float.


### PixelSizeOfSliceDimY ###

This is a float. 


### PrepareROIContrasts ###

```
document.PrepareROIContrasts(a)
```

a : int
:	the number of predictors


### Remove ###

```
document.Remove()
```


### SDMContainsConstantPredictor ###

This is a bool.


### Save ###

```
x = document.Save()
```

x : bool
:	success (`True` or `False`)


### SaveAs ###

```
x = document.SaveAs(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### SaveFMRAndSTCFromMem ###

```
x = document.SaveFMRAndSTCFromMem(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### SaveGLM ###

```
document.SaveGLM(a)
```

a : str
:	the file name


### SaveMesh ###

```
x = document.SaveMesh(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### SaveMultiStudyGLMDefinitionFile ###

```
document.SaveMultiStudyGLMDefinitionFile(a)
```

a : str
:	the file name


### SaveSingleStudyGLMDesignMatrix ###

```
document.SaveSingleStudyGLMDesignMatrix(a)
```

a : str
:	the file name


### SaveSnapshotOfSurfaceWindow ###

```
x = document.SaveSnapshotOfSurfaceWindow(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### SaveStimulationProtocol ###

```
document.SaveStimulationProtocol(a)
```

a : str
:	the file name


### SaveVTC ###

```
x = document.SaveVTC(a)
```

a : str
:	the file name

x : bool
:	success (`True` or `False`)


### SaveVolumeMaps ###

```
document.SaveVolumeMaps(a)
```

a : str
:	the file name


### ScalePredictorValues ###

```
document.ScalePredictorValues(a, b, c)
```

a : str
:	the predictor name

b : float
:	the new maximum value

c : bool
:	scale only if values are positive (`True` or `False`)


### SelectVOI ###

```
document.SelectVOI(a)
```

a : int
:	the VOI index


### SeparationOfStudyPredictors ###

This is a bool.


### SeparationOfSubjectPredictors ###

This is a bool.


### SetConditionColor ###

```
document.SetConditionColor(a, b, c, d)
```

a : str
:	the condition name

b : int
:	the red colour level

c : int
:	the green colour level

d : int
:	the blue colour level


### SetContrastString ###

```
document.SetContrastString(a)
```

a : str
:	the contrast string


### SetContrastValue ###

```
document.SetContrastValue(a, b)
```

a : str
:	the predictor name

b : int
:	the contrast value


### SetContrastValueAtIndex ###

```
document.SetContrastValueAtIndex(a, b)
```

a : int
:	the predictor index

b : int
:	the contrast value


### SetCurrentContrast ###

```
document.SetCurrentContrast(a)
```

a : str
:	the contrast name


### SetCurrentContrastAtIndex ###

```
document.SetCurrentContrastAtIndex(a)
```

a : int
:	the contrast index


### SetPredictorValues ###

```
document.SetPredictorValues(a, b, c, d)
```

a : str
:	the predictor name

b : int
:	the interval start

c : int
:	the interval end

d : float
:	the predictor value


### SetPredictorValuesFromCondition ###

```
document.SetPredictorValuesFromCondition(a, b, c)
```

a : str
:	the predictor name

c : str
:	the protocol condition name

d : float
:	the predictor value


### SetVoxelIntensity ###

```
document.SetVoxelIntensity(a, b, c, d)
```

a : int
:	the x coordinate

b : int
:	the y coordinate

c : int
:	the z coordinate

d : int
:	the intensity value


### ShowGLM ###

```
document.ShowGLM()
```


### ShowSelectedVOIs ###

```
document.ShowSelectedVOIs()
```


### ShowVolumeMap ###

```
document.ShowVolumeMap(a)
```

a : int
:	the volume map index


### ShowVolumeMapsDlg ###

```
document.ShowVolumeMapsDlg()
```


### SliceThickness ###

This is a float.


### SliceTimeCorrection ###

```
x = document.SliceTimeCorrection(a)
```

a : int
:	the slice order (0: Ascending, 1: Ascending-interleaved,
    2: Ascending-interleaved 2 (Siemens only), 10: Descending,
    11: Descending-interleaved, 12: Descending-interleaved 2)

x : bool
:	success (`True` or `False`)


### SpatialGaussianSmoothing ###

```
x = document.SpatialGaussianSmoothing(a, b)
```

a : float
:	the FWHM value

b : str
:	the FWHM value unit ("mm" or "px")

x : bool
:	success (`True` or `False`)


### StimulationProtocolBackgroundColorB ###

This is a int.


### StimulationProtocolBackgroundColorG ###

This is a int.


### StimulationProtocolBackgroundColorR ###

This is a int.


### StimulationProtocolExperimentName ###

This is a str.


### StimulationProtocolFile ###

This is a str.


### StimulationProtocolResolution ###

This is an int.


### StimulationProtocolTextColorB ###

This is an int.


### StimulationProtocolTextColorG ###

This is an int.


### StimulationProtocolTextColorR ###

This is an int.


### StimulationProtocolTimeCourseColorB ###

This is an int.


### StimulationProtocolTimeCourseColorG ###

This is an int.


### StimulationProtocolTimeCourseColorR ###

This is an int.


### StimulationProtocolTimeCourseThickness ###

This is an int.


### TR ###

This is an int.


### TargetVTCBoundingBoxXEnd ###

This is an int.


### TargetVTCBoundingBoxXStart ###

This is an int.


### TargetVTCBoundingBoxYEnd ###

This is an int.


### TargetVTCBoundingBoxYStart ###

This is an int.


### TargetVTCBoundingBoxZEnd ###

This is an int.


### TargetVTCBoundingBoxZStart ###

This is an int.


### TimeResolutionVerified ###

This is a bool.


### TemporalGaussianSmoothing ###

```
x = document.TemporalGaussianSmoothing(a, b)
```

a : float
:	the FWHM value

b : str
:	the FWHM value unit ("mm" or "px")

x : bool
:	success (`True` or `False`)


### TemporalHighPassFilter ###

```
x = document.TemporalHighPassFilter(a, b)
```

a : float
:	the highpass value

b : str
:	the highpass value unit ("cycles" or "Hz")

x : bool
:	success (`True` or `False`)


### TemporalHighPassFilterGLMDCT ###

```
x = document.TemporalHighPassFilterGLMDCT(a)
```

a : int
:	the number of basis functions

x : bool
:	success (`True` or `False`)


### TemporalHighPassFilterGLMFourier ###

```
x = document.TemporalHighPassFilterGLMFourier(a)
```

a : int
:	the number of cycles

x : bool
:	success (`True` or `False`)


### UpdateSurfaceWindow ###

```
document.UpdateSurfaceWindow()
```


### UpdateWindow ###

```
document.UpdateWindow(a)
```

a : bool (optional)
:	process events (`True` or `False`)


### UseBoundingBoxForVTCCreation ###

This is a bool.


### VMRVoxelResolutionX ###

This is a float.


### VMRVoxelResolutionY ###

This is a float.


### VMRVoxelResolutionZ ###

This is a float.


### VoxelResolutionVerified ###

This is a bool.


### ZTransformStudies ###

This is a bool.


### ZTransformStudiesBaselineOnly ###

This is a bool.


### blockSignals ###

```
x = document.blockSignals(a)
```

a : bool
:	`True` or `False`

x : bool
:	state before change (`True` or `False`)


### childEvent ###

```
document.childEvent(a, b)
```

a : QChildEvent
:	?

b : ?
:	?


### children ###

```
x = document.children()
```

x : tuple
:	?


### className ###

```
x = document.className()
```

x : str
:	`'BrainVoyagerScriptAccess'`


### connect ###

```
x = document.connect(a, b, c, d, e)
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
document.customEvent(a, b)
```

a : QEvent
:	?

b : ?
:	?


### delete ###

```
document.delete()
```


### deleteLater ###

```
document.deleteLater()
```


### destroyed ###

```
document.distroyed()
```


### disconnect ###

```
x = document.disconnect(a, b, c, d)
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
document.dumpObjectInfo(a)
```

a : ?
:	?


### dumpObjectTree ###

```
document.dumpObjectTree(a)
```

a : ?
:	?

 
### dynamicPropertyNames ###

```
document.dynamicPropertyNames(a)
```

a : ?
:	?

 
### event ###

```
x = document.event(a)
```

a : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### eventFilter ###

```
x = document.eventFilter(a, b)
```

a : QObject (?)
:	?

b : QEvent (?)
:	the event

x : bool
:	`True` or `False`


### findChild ###

```
x = document.findChild(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : QObject (?)
:	the child


### findChildren ###

```
x = document.findChildren(a, b)
```

a : PyObject (?)
:	?

b : str
:	the name (?)

x : tuple
:	the children


### help ###

```
document.help()
```


### inherits ###

```
document.inherits()
```


### installEventFilter ###

```
document.installEventFilter(a)
```

a : QObject (?)
:	?


### isSignalConnected ###

```
x = document.isSignalConnected(a)
```

a : QMethodSignal (?)
:	the signal

x : bool
:	`True` or `False`


### isWidgetType ###

```
x = document.isWidgetType()
```

x : bool
:	`True` or `False`


### isWindowType ###

```
x = document.isWindowType()
```

x : bool
:	`True` or `False`


### killTimer ###

```
document.killTimer(a)
```

a : int
:	the id


### metaObject ###

```
x = document.metaObject()
```

x : PythonQt.QtCore.QMetaObject (?)
:	?


### moveToThread ###

```
document.moveToThread(a)
```

a : QThread
:	the thread


### objectName ###

This is a str.


### objectNameChanged ###

```
document.objectNameChanged(a)
```

a : str (?)
:	?


### parent ###

```
x = document.parent()
```

x : QObject (?)
:	?


### property ###

```
x = document.property(a)
```

a : str (?)
:	the name

x : ?
:	?


### removeEventFilter ###

```
document.removeEventFilter(a)
```

a : QObject (?)
:	?


### sender ###

```
document.sender()
```

x : QObject (?)
:	?


### senderSignalIndex ###

```
document.senderSignalIndex()
```

x : int
:	the index


### setObjectName ###

```
document.setObjectName(a)
```

a : str
:	the name


### setParent ###

```
document.setParent(a)
```

a : QObject
:	the parent


### setProperty ###

```
document.setProperty(a)
```

a : str (?)
:	the property name

b : ?
:	the property value


### signalsBlocked ###

```
x = document.signalsBlocked()
```

x : bool
:	`True` or `False`


### startTimer ###

```
x = document.startTimer(a)
```

a : int
:	the interval

b : QT::TimeType (?)
:	the timer type (?)

x : int
:	?


### thread ###

```
document.thread()
```


### timerEvent ###

```
document.timerEvent(a)
```

a : QTimerEvent (?)
:	?


### tr ###

```
x = document.tr(a, b, c)
```

a : QByteArray (?)
:	?

b : QByteArray (?)
:	?

c : int
:	?

x : str
:	?


### vmp_dims ###

```
x = document.vmp_dims()
```

x : tuple
:	?
