set(target ${MP2_CUSTOM_PROJECT})

project(${target})

file(GLOB hdrs "*.h*")
file(GLOB srcs "${CMAKE_CURRENT_SOURCE_DIR}/src/*.cpp*")

#add_custom_target(${target} SOURCES ${hdrs})


add_custom_target(${target} ${hdrs} ${srcs})