cmake_minimum_required(VERSION 3.16)
project(gci2raw)

set(CMAKE_CXX_STANDARD 17)

include_directories(src)

add_executable(gci2raw
        src/main.cpp
        src/GCMemcard.cpp
        src/Common/NandPaths.cpp
        src/Common/Timer.cpp
        src/Common/StringUtil.cpp
        src/Common/ColorUtil.cpp
        src/Common/CommonFuncs.cpp
        src/Common/File.cpp
        src/Common/MsgHandler.cpp
        src/Core/HW/EXI/EXI_Device.cpp
        src/Core/HW/EXI/EXI_DeviceIPL.cpp
        src/Core/HW/Sram.cpp)
