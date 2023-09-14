set(target_name basic)
add_library(${target_name} STATIC "")
target_sources(${target_name}
    PRIVATE "${PROJECT_SOURCE_DIR}/src/basic/messages.cpp"
    PRIVATE "${PROJECT_SOURCE_DIR}/include/basic/messages.h"
)
target_include_directories(${target_name} 
    PUBLIC   
        "${PROJECT_SOURCE_DIR}/include"
        "${PROJECT_BINARY_DIR}"
)
