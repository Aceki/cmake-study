add_executable(sample_program main.cpp)

include_directories(../sample_lib) # Определяет дополнительные пути поиска заголовочных файлов компилятором.

target_link_libraries(sample_program sample_lib) # Определяет зависимость цели sample_program от sample_lib.
						 # Кроме того, команда устанавливет, что при построении цели sample_program будет
						 # использоваться библиотека, создаваемая в результате построения цели sample_lib.
