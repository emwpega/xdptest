project(xdptest CXX)

set(XDPTEST_SRC
    AfXdpUser.cpp
    )

add_executable(xdpuser
AfXdpUser.cpp
)
#target_link_libraries(xdpuser PUBLIC gsntrace ddevio general_classes)
#install(TARGETS xdpuser DESTINATION ${BUILD_DIR})
