cmake_minimum_required(VERSION 3.17)

project(CW2022MiniWorkshop)

find_program(PANDOC pandoc)

add_custom_target(slides ALL
    COMMAND
    ${PANDOC} -s slides.md -o ${CMAKE_BINARY_DIR}/slides.html
    -t revealjs
    -V revealjs-url=reveal.js
    -V theme=white
    WORKING_DIRECTORY ${CMAKE_SOURCE_DIR}
    DEPENDS ${CMAKE_SOURCE_DIR}/slides.md
    )

file(COPY ${CMAKE_SOURCE_DIR}/img DESTINATION ${CMAKE_BINARY_DIR})
