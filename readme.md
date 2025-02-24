# Installation

### Requirements for Windows
- Git
- Visual Studio 2022 with CMake and Ninja

- Open PowerShell and execute this command to get the correct environment:
```powershell
& 'C:\Program Files\Microsoft Visual Studio\2022\Community\Common7\Tools\Launch-VsDevShell.ps1' -SkipAutomaticLocation -Arch amd64
```

### Commands

```batch
git clone --recurse-submodules --shallow-submodules https://github.com/dsa-t/openEMS-Project --branch custom -j 16
cd openEMS-Project
git -C CSXCAD fetch --prune --unshallow --tags
git -C openEMS fetch --prune --unshallow --tags
mkdir build
cd build
cmake -GNinja -DCMAKE_INSTALL_PREFIX=C:\Sim\Prefix ..
cmake --build . -j 16
```

---

 ![openEMS](https://raw.github.com/thliebig/openEMS-Project/master/other/openEMS.png "openEMS")<br />
openEMS is a free and open electromagnetic field solver using the FDTD method. Octave/Matlab and Python used as an easy and flexible scripting interface.<br />

**Website**: [https://openEMS.de](https://openEMS.de)<br />
**Documentation**: [https://docs.openEMS.de](https://docs.openEMS.de)<br />
**Github**: [https://github.com/thliebig/openEMS-Project](https://github.com/thliebig/openEMS-Project)<br />

# openEMS Features:
+ fully 3D Cartesian and cylindrical coordinates graded mesh.
+ Multi-threading, SIMD (SSE) and MPI support for high speed FDTD.
+ Octave/Matlab and Pyhon-Interface
+ Dispersive material (Drude/Lorentz/Debye type)
+ Field dumps in time and frequency domain as vtk or hdf5 file format
+ Flexible post-processing routines in Octave/Matlab and Python
+ and [many more](http://openems.de/index.php/OpenEMS#Features)

# Install Instruction

[https://docs.openems.de/install.html](https://docs.openems.de/install.html)

