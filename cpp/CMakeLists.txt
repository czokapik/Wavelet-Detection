cmake_minimum_required(VERSION 3.20)
project(WaveletDetection)

set(CMAKE_CXX_STANDARD 17)

# Szukaj OpenCV (je�li nie znajdzie, poka�e b��d)
find_package(OpenCV REQUIRED)

# Dodaj pliki �r�d�owe
add_executable(${PROJECT_NAME} 
    src/main.cpp
 )

# Pod��cz OpenCV
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})