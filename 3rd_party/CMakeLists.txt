add_subdirectory(glad)
add_subdirectory(glfw)

add_library(third-party INTERFACE)

target_link_libraries(third-party INTERFACE
    glad
    glfw
)

