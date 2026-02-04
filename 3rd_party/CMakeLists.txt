add_subdirectory(glad)
add_subdirectory(glfw)
add_subdirectory(glm)
add_subdirectory(entt)

add_library(3rd_party INTERFACE)

target_link_libraries(3rd_party INTERFACE
    glad
    glfw
    glm
    EnTT
)
