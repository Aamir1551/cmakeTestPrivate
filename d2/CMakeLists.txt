project(d2)

add_library(h "d3/hh.hpp")
add_library(i "ii.hpp" "j.cpp")
target_link_libraries(i h)
target_include_directories(i PRIVATE "d3") #try wtih private

set_target_properties(i PROPERTIES LINKER_LANGUAGE CXX)
set_target_properties(h PROPERTIES LINKER_LANGUAGE CXX)