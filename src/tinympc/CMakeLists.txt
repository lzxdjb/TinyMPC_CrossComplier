
add_library(tinympc 
    admm.cpp
    # codegen.cpp
)

target_include_directories(tinympc PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/..) 

