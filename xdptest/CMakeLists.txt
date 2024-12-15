project(xdptest C)

#set(xdpuser_SRC
#    AfXdpUser.cpp
#    )

#set(xdpuser_INCLUDE
#  PRIVATE
#    ../xdp-tools/headers
#    ./xdp-tools/headers/xdp
#  )

add_executable(xdpuser
AfXdpUser.c
)

target_include_directories(xdpuser
  PUBLIC
    ../xdp-tools/headers
 #   ./xdp-tools/headers/xdp
  )

#target_compile_options(xdpuser PRIVATE -Wno-write-strings)

target_link_libraries(xdpuser PUBLIC common libbpf.a)
#install(TARGETS xdpuser DESTINATION ${BUILD_DIR})
