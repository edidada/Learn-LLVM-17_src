cmake_minimum_required (VERSION 3.22.0)

project(LearnLLVM17 LANGUAGES CXX C)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
find_package(LLVM 17 REQUIRED CONFIG)

message(STATUS "Found LLVM ${LLVM_PACKAGE_VERSION}")
message(STATUS "LLVM CMake dir: ${LLVM_DIR}")

include(AddLLVM)   # 这一行定义了 llvm_add_library

include_directories(${LLVM_INCLUDE_DIRS})
add_definitions(${LLVM_DEFINITIONS})

add_subdirectory ("Chapter02/calc")
#add_subdirectory ("Chapter03/tinylang")
#add_subdirectory ("Chapter04/tinylang")
add_subdirectory ("Chapter05/tinylang")
#add_subdirectory ("Chapter06/calc")
#add_subdirectory ("Chapter06/tinylang")
#add_subdirectory ("Chapter07/ppprofiler")
#add_subdirectory ("Chapter07/tinylang")
#add_subdirectory ("Chapter07/tinylang2")
#add_subdirectory ("Chapter08/TableGen")
#add_subdirectory ("Chapter09/jit")
#add_subdirectory ("Chapter09/lljit")