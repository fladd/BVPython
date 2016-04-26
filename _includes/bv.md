bv
==


### fmrarray_t ###

Get volume for specified time point t of FMR document as a contigous 1D numpy array.
**Note**: This provides direct access to the original (float32) memory block (no copy).

```
x = bv.fmrarray_t(a, b)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : int
:	the time point

x : numpy.ndarray
:	the volume data


### mesharrays ###

Get three arrays of the x, y, z coordinates of the vertices of a mesh (SRF) document as contigous 1D numpy arrays.
**Note**: This function provides direct access to the original (float32) memory blocks (no copy).
    
```
x, y, z = bv.mesharrays(a)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

x : numpy.ndarray
:	the x coordinates of the vertices of the mesh

y : numpy.ndarray
:	the y coordinates of the vertices of the mesh

z : numpy.ndarray
:	the z coordinates of the vertices of the mesh


### set_fmrarray_t ###

Sets the values of the volume for the specified time point t of FMR document from provided float32 numpy array.

```
x = bv.set_fmrarray_t(a, b ,c)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : int
:	the time point

c : numpy.ndarray
:	The values of the volume

x : bool
:	success (`True` or `False`)


### set_mesharrays ###

Sets the values of the x, y, z coordinates of the vertices of a mesh (SRF) document from 3 provided float32 numpy arrays.

```
x = bv.set_mesharrays(a, b, c, d)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:   the document

b : numpy.ndarray
:	The values of the x coordinates of the vertices of the mesh

c : numpy.ndarray
:	The values of the y coordinates of the vertices of the mesh

d : numpy.ndarray
:	The values of the z coordinates of the vertices of the mesh

x : bool
:	success (`True` or `False`)


### set_smparray_i ###

Sets the values of surface map specified with index i of hosting VMR-SRF document from provided float32 numpy array.

```
x = bv.set_smparray_i(1, b, c)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : int
:	the index

c : numpy.ndarray
:	The values of the surface map

x : bool
:	success (`True` or `False`)


### set_vmparray_i ###

Sets the values of volume map specified with index i of hosting VMR document from provided float32 numpy array.

```
x = bv.set_vmparray_i(a, b, c)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : int
:	the index

c : numpy.ndarray
:	The values of the volume map

x : bool
:	success (`True` or `False`)


### set_vrmarray ###

Sets the values of the volume of VMR document from provided uint8 numpy array.

```
x = bv.set_vmrarray(a, b, c)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : numpy.ndarray
:	The values of the volume

x : bool
:	success (`True` or `False`)


### smparray_i ###

Get surface map for specified index i of hosting VMR-SRF document as a contigous 1D numpy array.
**Note**: This function provides direct access to the original (float32) memory block (no copy).
    
```
x = bv.smparray_i(a, b)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : int
:	the index

x : numpy.ndarray
:	the surface map


### vmparray_i ###

Get volume map for specified index i of hosting VMR document as a contigous 1D numpy array.
**Note**: This provides direct access to the original (float32) memory block (no copy).
    
```
x = bv.vmparray_i(a, b)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

b : int
:	the index

x : numpy.ndarray
:	the volume map


### vmrarray ###

Get the volume of VMR document as a contigous 1D numpy array.
**Note**: This provides direct access to the original byte (uint8) memory block (no copy).

```
x = bv.vmparray_i(a)
```

a : [DocumentScriptAccess](./script_access.html#documentscriptaccess)
:	the document

x : numpy.ndarray
:	the volume map
