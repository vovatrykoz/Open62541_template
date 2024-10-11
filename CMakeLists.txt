cmake_minimum_required(VERSION 3.20)
project(open62541_template LANGUAGES C CXX)

set(PATH_TO_OPEN62541 ${PROJECT_SOURCE_DIR}/../open62541)
set(BUILD_PATH_FOR_OPEN62541 ${PROJECT_SOURCE_DIR}/../open62541)

set(CODE_SOURCE_DIR ${PROJECT_SOURCE_DIR}/source)

add_subdirectory(${PATH_TO_OPEN62541} ${BUILD_PATH_FOR_OPEN62541})

add_executable(
    exampleRunner
    ${CODE_SOURCE_DIR}/main.cpp
)

target_compile_features(exampleRunner PUBLIC cxx_std_17)
target_link_libraries(exampleRunner open62541::open62541)