cmake_minimum_required(VERSION 3.0)
project(zad6)

add_library(test6 SHARED <src>)
install(TARGETS test6 DESTINATION <dir1>)

link_directories(<dir1>)

add_executable(myProg)
install(TARGETS myProg DESTINATION <dir2>)

target_link_libraries(myProg <dir1>/libtest6.dylib)