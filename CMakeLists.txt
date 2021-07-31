add_library(ik-ev ev.c)
target_include_directories(ik-ev PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}
    PRIVATE ${CMAKE_CURRENT_BINARY_DIR})
target_compile_definitions(ik-ev PUBLIC EV_STANDALONE=1 EV_CHILD_ENABLE=0)
