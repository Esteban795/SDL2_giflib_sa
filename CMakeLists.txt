cmake_minimum_required(VERSION 3.10)

set(SDL2_GIFLIB_SA_MODULE_SOURCES
    CEV_gifDeflate.c
    CEV_gifToSurface.c
    CEV_gifUser.c
    )

add_library(SDL2_giflib_sa STATIC ${SDL2_GIFLIB_SA_MODULE_SOURCES})

target_include_directories(SDL2_giflib_sa PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/)