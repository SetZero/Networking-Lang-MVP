message("Flex version: ${FLEX_VERSION}")
message("Bison version: ${BISON_VERSION}")

flex_target(${FlexName} test.lpp test.yy.cpp)
bison_target(${BisonName} test.ypp test-tab.cpp)

add_executable(fl ${FLEX_${FlexName}_OUTPUTS} ${BISON_${BisonName}_OUTPUTS})