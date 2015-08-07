cmake_minimum_required(VERSION 2.8)

project(git C)

add_compile_options(-ggdb)

add_executable(init-db init-db.c)
add_executable(update-cache update-cache.c read-cache.c)
add_executable(show-diff show-diff.c read-cache.c)
add_executable(write-tree write-tree.c read-cache.c)
add_executable(read-tree read-tree.c read-cache.c)
add_executable(commit-tree commit-tree.c  read-cache.c)
add_executable(cat-file cat-file.c read-cache.c)

target_link_libraries(init-db crypto z)
target_link_libraries(update-cache crypto z)
target_link_libraries(show-diff crypto z)
target_link_libraries(write-tree crypto z)
target_link_libraries(read-tree crypto z)
target_link_libraries(commit-tree crypto z)
target_link_libraries(cat-file crypto z)

add_custom_target(Documentation SOURCES README README.md)

