set(TARGET_NAME 02)

find_package(Eigen3 REQUIRED)
find_package(OpenCV REQUIRED)

add_executable(02 main.cpp rasterizer.hpp rasterizer.cpp global.hpp Triangle.hpp Triangle.cpp)

target_link_libraries(02  ${OpenCV_LIBS}  Eigen3::Eigen)
