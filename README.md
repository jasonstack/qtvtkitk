How to setup qt/vtk/itk on windows
======

Step 0: Set up files and forder hierarchy
------
- 0.1 Download qt 4.8/qt add-on /vtk 5.8/itk 3.2 /cmake 2.8
- 0.2 Create a folder called "qt-vtk-itk"  
- 0.3 Create "qt 4.8"/"vtk 5.8"/"itk 3.2" folders under "qt-vtk-itk"
- 0.4 Create "Src" forlder for each of 3 forlders
- 0.5 install qt 4.8 to the "qt 4.8" folder
- 0.6 unzip vtk 5.8 to the "vtk 5.8/src" folder
- 0.7 unzip itk 3.2  to the "itk 3.2/src" folder
- 0.8 install cmake
Step 1: Set up Qt
------
- 1.1 use visual studio 2010 command promt
- 1.2 navigate to the "qt 4.8" folder
- 1.3 type in "configure  –release -platform win32-msvc2010"
- 1.4 type in "nmake" ...(1-2hrs)
- 1.5 install qt add-on

Step 2: Set  up VTK
-------
- 2.1 open cmake, put source directory as "...../vtk 5.8/src/"
- 2.2 put binary directory as "..../vtk 5.8/bin/"
- 2.3 clicke "configure", choose VC10 as compiler
- 2.4 Enable "VTK_USE_QT", configure
- 2.5 Enable "VTK_USE_GUISUPPORT", configure
- 2.6 click "Generate"
- 2.7 go to "....../vtk 5.8/bin/" folder, user visual studio to open "vtk.sln"
- 2.8 build project in "Release" mode.. (cos we configure qt in release)

Step 3: Set  up ITK
-------
- 3.1 open cmake, put source directory as "...../itk 3.2/src/"
- 3.2 put binary directory as "..../itk 3.2/bin/"
- 3.3 clicke "configure", choose VC10 as compiler
- 3.4 click "Generate"
- 3.5 go to "....../itk 3.2/bin/" folder, user visual studio to open "itk.sln"
- 3.6 build project in "Release" mode.. (cos we configure qt in release)

THAT'S ALL
---------


--------











