include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)  # Includes the contents of the conanbuildinfo.cmake file.
conan_basic_setup()  # Prepares the CMakeList.txt for Conan.

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# $source_files is a space-delimited list of filenames.
add_executable(main main.cpp)  # Specifies the executable to build.
target_link_libraries(main ${CONAN_LIBS})  # Specifies what libraries to link, using Conan.