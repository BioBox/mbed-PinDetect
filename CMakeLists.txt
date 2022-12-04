
include(${MBED_PATH}/tools/cmake/app.cmake)

set(CMAKE_TRY_COMPILE_TARGET_TYPE "STATIC_LIBRARY")
set(MBED_PATH ${CMAKE_CURRENT_SOURCE_DIR}/../../os/mbed-os/ CACHE INTERNAL "")
set(MBED_CONFIG_PATH ${CMAKE_CURRENT_BINARY_DIR}/.. CACHE INTERNAL "")

add_library(pindetect PinDetect.h)
target_link_libraries(pindetect mbed-os)
set_target_properties(pindetect PROPERTIES LINKER_LANGUAGE CXX)
