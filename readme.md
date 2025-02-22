# Installation with vcpkg

## Windows

### Requirements
- Visual Studio 2022 with CMake and Ninja
- Git

### Commands in "Developer Command Prompt for VS 2022"

```batch
git config checkout.workers -1
git clone --recurse-submodules --shallow-submodules https://github.com/dsa-t/openEMS-Project --branch custom --depth 1 -j 16
cd openEMS-Project
mkdir build
cd build
cmake -GNinja -DCMAKE_BUILD_TYPE=RelWithDebInfo -DCMAKE_INSTALL_PREFIX=C:\Sim\Prefix ..
cmake --build . --config RelWithDebInfo -j 16
cmake --install .
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

