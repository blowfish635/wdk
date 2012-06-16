This repository contains tools and template files I created throughout time while using the WDK.

Take care the template files (sources, .sln, .vcxproj) contain placeholders marked with
\<\<explanation\>\> which must be edited on notepad for a template copy before it start to be used.

####\build\template\

*   Provide template build files for different kinds of projects: sys, exe, dll.

####\vs\2010\

*   Provide Visual Studio 2010 solution and project files to be used to build with the WDK build
    tool.

####\vs\2010\props\

*   Provide Visual Studio 2010 property sheets to load the build environments of each supported WDK
    build configuration.
    
    The property sheets use custom environment variables to refer to WDK installations instead of
    hardcoded paths, e.g.:  

*   *   Variable: WDK_6001_18002   - Sample value: C:\WDK\6001.18002  
        Variable: WDK_7600_16385_1 - Sample value: C:\WDK\7600.16385.1

    The __WDK_7600_16385_1__ variable refers to a __Windows Driver Kit for Windows 7__ installation,
    needed for most builds except the one for Windows 2000, which it doesn't
	support. The configuration for building for Windows 2000 will need a second WDK
	installation: __WDK for Windows Server 2008__.  
	This variables must be created and set properly, according with the WDK installation
	paths.

####\tools\

*   Provide some tools.  
    scd:  

*   *   This batch tool is used to navigate through short path names. Nice to use with the WDK for
        building in directories with spaces. Put it on your path.