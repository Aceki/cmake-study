# Пусть проект включает исполняемый файл и две библиотеки, которые он использует.

# В этом случае для формирования при построении системы выходных каталогов, совместимой с рекомендациями GNU,
# можно использовать следующее описани системы CMake.

project(my_project)

# Здесь специальная переменная CMAKE_BINARY_DIR хранит полный путь к каталогу построения проекта верхнего уровня.
# Вместо неё в этом примере можно использовать переменную CMAKE_CURRENT_BINARY_DIR, в которой хранится
# путь к каталогу построени текущего (под)проекта.
set(BINARY_DIR "${CMAKE_BINARY_DIR}")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${BINARY_DIR}/bin")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${BINARY_DIR}/lib")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${BINARY_DIR}/lib")



add_subdirectory(my_library_1)
add_subdirectory(my_library_2)
add_subdirectory(my_program)
