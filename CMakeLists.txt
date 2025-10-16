cmake_minimum_required(VERSION 3.13)

add_library(tud_xinput INTERFACE)
target_sources(tud_xinput INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/tud_xinput.c
)
target_include_directories(tud_xinput INTERFACE
 ${CMAKE_CURRENT_LIST_DIR}
)
target_link_libraries(tud_xinput INTERFACE tinyusb)
