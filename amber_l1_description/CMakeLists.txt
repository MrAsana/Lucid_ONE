cmake_minimum_required(VERSION 3.5)
project(amber_l1_description)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY config meshes launch urdf
  DESTINATION share/${PROJECT_NAME}
)

#ament_environment_hooks("${CMAKE_CURRENT_SOURCE_DIR}/env-hooks/${PROJECT_NAME}.dsv.in")

ament_package()
