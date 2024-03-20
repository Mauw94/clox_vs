# CMakeList.txt : CMake project for clox_vs, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (clox_vs "clox_vs.c" "clox_vs.h" "common.h" "chunk.h" "memory.h" "debug.h" "chunk.c" "memory.c" "debug.c" "value.h" "value.c" "vm.h" "vm.c" "compiler.h" "compiler.c" "scanner.h" "scanner.c")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET clox_vs PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
