project(TemplateProject_src)

include_directories(../include)

set(SOURCE_FILES TemplateProject.cpp)

add_library(TemplateProject_src STATIC ${SOURCE_FILES})