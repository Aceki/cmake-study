add_library(my_lib my_lib.cpp my_lib.h)

target_include_directories(my_lib INTERFACE .) # "." - текущий каталог
