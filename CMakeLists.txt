cmake_minimum_required (VERSION 3.8 FATAL_ERROR)

set(PROJECT_NAME SlaveBot)

project (${PROJECT_NAME})

add_subdirectory(SlaveBotCore)
add_subdirectory(SlaveBotEditor)

set_property(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR} PROPERTY VS_STARTUP_PROJECT SlaveBotEditor)
