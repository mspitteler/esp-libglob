
list(APPEND srcs glob.c)

idf_component_register(SRCS ${srcs}
                       INCLUDE_DIRS ".")

target_compile_options(${COMPONENT_LIB} PRIVATE -Dlstat=stat -O2)
