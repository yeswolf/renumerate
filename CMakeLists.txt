cmake_minimum_required(VERSION 3.17)
project(reenumerate)

add_executable(reenumerate reenumerate.c)
target_link_libraries(reenumerate "-framework IOKit" "-framework CoreFoundation")
install(TARGETS reenumerate DESTINATION bin)
