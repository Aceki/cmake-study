#Пусть необходимо построить проект, содержащий две цели: статическую библиотеку и приложение, использующее эту библиотеку.

set(BUILD_SHARED_LIBS FALSE) # Включает построение статических библиотек.

cmake_minimum_required(VERSION 2.8) # Устанавливает наименьшую версию CMake, которым можеть быть обработан проект.

project(lib)

add_subdirectory(sample_lib) # Присоединяем проект нижнего уровня.
add_subdirectory(sample_program)
