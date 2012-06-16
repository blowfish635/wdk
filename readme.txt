This repository contains tools and template files I created throughout time while using the WDK.

Take care the template files (sources, .sln, .vcxproj) contain placeholders marked with
&lt;&lt;explanation&gt;&gt; which must be edited on notepad for a template copy before it start to be used.

####\build\template\

*   Provide template build files for different kinds of projects: sys, exe, dll.

####\vs\2010\

*   Provide Visual Studio 2010 solution and project files to be used to build with the WDK build
    tool.

####\vs\2010\props\

*   Provide Visual Studio 2010 property sheets to load the build environments of each supported WDK
    build configuration.

####\tools\

*   Provide some tools.

*   scd:

*   *   This batch tool is used to navigate through short path names. Nice to use with the WDK for
        building in directories with spaces. Put it on your path.