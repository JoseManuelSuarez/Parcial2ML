cmake_minimum_required(VERSION 3.5)

project(RegresionLineal LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

#Se incluye el directorio de: eigen
#include_directories("/usr/include/eigen3")

#Se crea una lista con todas las fuentes .cpp
set(project_sources
    main.cpp
    extoeigen.cpp
    modellinealregresion.cpp
    )
#Se crean los ejecutables con todos los archivos fuentes necesarios
add_executable(${PROJECT_NAME}
    ${project_sources})
