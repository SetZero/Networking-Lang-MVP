cmake_minimum_required (VERSION 3.20)
project (network_lang)

find_package(BISON)
find_package(FLEX)

set(FlexName linter)
set(BisonName parser)

add_subdirectory(src)