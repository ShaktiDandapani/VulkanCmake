cmake_minimum_required(VERSION 3.17)

include_directories(${CMAKE_SOURCE_DIR}/include)
link_directories(${CMAKE_SOURCE_DIR}/libs)

add_executable(vulkan_run vulk_main.cpp)

# find_package(OpenGL REQUIRED)

target_link_libraries(vulkan_run 
                      glfw3.lib
                      vulkan-1.lib
                      )