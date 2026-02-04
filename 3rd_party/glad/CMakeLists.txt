cmake_minimum_required(VERSION 3.24)

# Create glad library
add_library(glad STATIC
    src/gl.c
)

# Set include directories
target_include_directories(glad PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include
)

# Ensure C11 standard
set_target_properties(glad PROPERTIES
    C_STANDARD 11
    C_STANDARD_REQUIRED ON
)
