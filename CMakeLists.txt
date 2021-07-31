configure_file(config.h.in config.h)
add_library(ik-ev ev.c)
target_include_directories(ik-ev PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}
    PRIVATE ${CMAKE_CURRENT_BINARY_DIR})