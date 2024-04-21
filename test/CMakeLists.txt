# set ( CMAKE_C_FLAGS "-Os -g -Wall -ffunction-sections")
# set ( STACK_SIZE 0xf00 )
# # set ( TARGET test )
# # set ( SRC_MODULES test startup dummy)
# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -mcmodel=medany")


add_executable(test1 test1.cpp)

# SET(LINKER_SCRIPT "${CMAKE_CURRENT_SOURCE_DIR}/test.lds")

target_link_libraries(test1 LINK_PUBLIC tinympc )

# SET(CMAKE_EXE_LINKER_FLAGS  "${CMAKE_EXE_LINKER_FLAGS} -nostartfiles   -fno-exceptions  -Xlinker --defsym=__stack_size=${STACK_SIZE} -T ${LINKER_SCRIPT} -Wl,-Map=${TARGET}.map")
