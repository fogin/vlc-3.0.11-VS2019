build help:

need install VS2019£º
1:  install  Visual Studio 2019 version 16.8 Preview 3
2:  Download the "Insider Preview Windows 10 SDK" and install to support C11/C17 feature. (now Windows SDK Version is 10.0.20206.0, reference https://devblogs.microsoft.com/cppblog/c11-and-c17-standard-support-arriving-in-msvc/ )

build step:
1: go to libs\x64, unpack libs_part_1.rar libs_part_2.rar to current folder
2: open winvlc.sln with VS2019
3: select Debug && x64
4：add macro _SILENCE_STDEXT_HASH_DEPRECATION_WARNINGS  in hash.h from libprotobuf
5: build contrib first, those are 3rd libs.
6: build winvlc project, it will auto build libcompat¡¢libvlc¡¢libvlccore project.
7. upgrade c++ lang standard in stream_out_chromecast project
6: build all plugins.
7: the output runable vlc is in  vlc-3.0.11-VS2019\x64\Debug\vlc



email:  niozhao@qq.com
