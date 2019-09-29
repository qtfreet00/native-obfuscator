# For more information about using CMake with Android Studio, read the
# documentation: https://d.android.com/studio/projects/add-native-code.html

# Sets the minimum version of CMake required to build the native library.

cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)

set(CLASS_FILES $classfiles)
set(MAIN_FILES $mainfiles)
add_library($projectname SHARED ${CLASS_FILES} ${MAIN_FILES})
