cmake_minimum_required( VERSION 3.20...4.2 )

project(monitor-core)

# ------------------------------------------------------------
# LIBRARIES
### add_library(shared-log SHARED src/log/log_agent.cpp)
### target_include_directories(shared-log PUBLIC ${PROJECT_SOURCE_DIR}/include PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})

# ------------------------------------------------------------
# TESTS
### add_executable(test-log-agent tests/unit/log/test_log_agent.cpp)
### target_link_libraries(test-log-agent PRIVATE shared-log gtest gtest_main)

## CMake testing with GoogleTest
### enable_testing()
### add_test(NAME LogAgent COMMAND test-log-agent)