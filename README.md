
## Create and connect a Visual Studio C++ project with openCL sdk and C++ bindings



## Steps

1) Download the openCL folder
2) Create a empty C++ Visual Studio Project. 
3) Create a source C++ file
4) Click on the project and go to Properties -> Configuration Properties -> C/C++ -> General 
5) Click on "Additional Include Directories" and add the path to the CL folder. (..\OpenCL\include)
6) Now go to Properties -> Configuration Properties -> Linker -> Input 
7) Click on "Additional Dependencies" and add "OpenCL.lib" to the other dependencies. Using a ";" to separate it from the others.
8) Now go to Properties -> Configuration Properties -> Linker -> General
9) Click on  "Additional Library Directories" and add the path to the OpenCL.lib file. (..\OpenCL\lib)
10) Now include in your file:
  #include <Cl/cl.hpp>
  #include <CL/opencl.h>
  
 
This should be it!

