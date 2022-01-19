cmake_minimum_required(VERSION 3.20)
project(project2_in_windows C)

set(CMAKE_C_STANDARD 11)

add_executable(project2_in_windows plane.c
        resource.c resource.h
        event.c event.h
        global.h
        main-function.c main-function.h
        )
target_link_libraries(plane mingw32)
target_link_libraries(plane SDL2main)
target_link_libraries(plane SDL2)
target_link_libraries(plane SDL2_image)

