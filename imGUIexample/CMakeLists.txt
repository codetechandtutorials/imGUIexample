cmake_minimum_required (VERSION 3.8)

add_executable (imGUIexample "imGUIexample.cpp" "UseImGui.cpp" "UseImGui.h")

find_package(glad CONFIG REQUIRED)
target_link_libraries(imGUIexample PRIVATE glad::glad)

find_package(glfw3 CONFIG REQUIRED)
target_link_libraries(imGUIexample PRIVATE glfw)

find_package(imgui CONFIG REQUIRED)
target_link_libraries(imGUIexample PRIVATE imgui::imgui)