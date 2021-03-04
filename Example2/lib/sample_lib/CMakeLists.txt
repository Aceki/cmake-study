# Сборка должна привести к созданию статической библиотеки в выходном каталоге проекта sample_lib.
# Имя файла библиотеки будет по умолчанию совпадать с именем цели sample_lib с префиксом и расширением, зависящим от компилятора.

#add_library(sample_lib STATIC sample_module.cpp sample_module.h)

add_library(sample_lib sample_module.cpp sample_module.h)
