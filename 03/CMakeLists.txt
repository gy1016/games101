set(TARGET_NAME 02)

find_package(Eigen3 CONFIG REQUIRED)
find_package(OpenCV REQUIRED)

add_executable(03 main.cpp rasterizer.hpp rasterizer.cpp global.hpp Triangle.hpp Triangle.cpp Texture.hpp Texture.cpp Shader.hpp OBJ_Loader.h)

target_link_libraries(03  ${OpenCV_LIBS}  Eigen3::Eigen)