add_executable(${PROJECT_NAME})
target_sources(${PROJECT_NAME} PRIVATE main.cpp)

file(GLOB_RECURSE SRC_FILES ${CMAKE_CURRENT_SOURCE_DIR}/*.cpp)

target_sources(${PROJECT_NAME} PRIVATE ${SRC_FILES})

target_link_libraries(${PROJECT_NAME} PRIVATE 3rd_party)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
