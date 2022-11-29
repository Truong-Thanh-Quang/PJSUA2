# PJSUA2
Building native lib PJSUA2.DLL

1) Run swig to generate .cs & cpp files (wrapper)
  - Download swig (https://www.swig.org/download.html)
  - Set the environment PATH to the directory containing swig.exe
  - Using a command prompt, change to the "pjsip-apps/src/swig/csharp" folder (or create the "csharp" sub-folder if it is missing)
  - Run commnd: _swig -I../../../../pjlib/include -I../../../../pjlib-util/include -I../../../../pjmedia/include -I../../../../pjsip/include -I../../../../pjnath/include -w312 -c++ -csharp -o pjsua2_wrap.cpp ../pjsua2.i_
2) Build pjsua2
- Edit PropertySheet.props: Change path to pjproject root folder, for example _<PJPROJECT_SRC_PATH>D:\Temp\pjproject\</PJPROJECT_SRC_PATH>_
- Open solution, build
