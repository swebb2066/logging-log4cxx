# Configure the resource file
# Note: On Windows, clang tries to compile the resource file, but it fails.
# Ignore it for now.
if(WIN32 AND CMAKE_CXX_COMPILER_ID STREQUAL "MSVC")
target_sources(log4cxx
  PRIVATE
  ../resources/log4cxx.rc
)
endif()
