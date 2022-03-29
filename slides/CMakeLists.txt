cmake_minimum_required(VERSION 3.17)

project(CW2022MiniWorkshop)

find_program(PANDOC pandoc)

add_custom_target(slides ALL
    COMMAND
    ${PANDOC} -s ${CMAKE_SOURCE_DIR}/slides.md
    -o ${CMAKE_BINARY_DIR}/slides.html
    -t revealjs
    -V revealjs-url=${CMAKE_SOURCE_DIR}/reveal.js
    -V theme=white
    DEPENDS ${CMAKE_SOURCE_DIR}/slides.md
    )
