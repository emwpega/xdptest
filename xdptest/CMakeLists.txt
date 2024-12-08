project(xdptest CXX)

set(XDPTEST_SRC
    Main.cpp
    )

add_executable(xdpuser
Main.cpp
)
#target_link_libraries(xdpuser PUBLIC gsntrace ddevio general_classes)
#install(TARGETS xdpuser DESTINATION ${BUILD_DIR})
