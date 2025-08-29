cmake_minimum_required(VERSION 4.0)

project(vk-test VERSION 0.1 LANGUAGES CXX)

find_package(glfw3 REQUIRED)
find_package(Vulkan REQUIRED)
find_package(glm REQUIRED)

add_executable(vk-test
	src/main.cpp
)

target_link_libraries(vk-test glfw)
target_link_libraries(vk-test vulkan)
target_link_libraries(vk-test glm)
