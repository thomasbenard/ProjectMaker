include_directories(
        ../lib/googletest/include
        ../lib/googletest
        ../lib/googlemock/include
        ../lib/googlemock/
        ../../include)

set(SOURCE_FILES TemplateProject_test.cpp )
add_executable(run_unittests ${SOURCE_FILES})

set(GMOCK_LIB_PATH /cygdrive/d/workspace/googletest/build_gmock/googlemock)
target_link_libraries(run_unittests gtest gtest_main gmock)
target_link_libraries(run_unittests TemplateProject_src)