project(common C)

set(common_SRC
    common_params.c
    common_user_bpf_xdp.c
    )

set(common_INCLUDE
  PUBLIC
    "${CMAKE_CURRENT_SOURCE_DIR}"
    ../xdp-tools/headers
  )

add_library(common SHARED ${common_SRC})

target_include_directories(common ${common_INCLUDE})

install(TARGETS common DESTINATION ../build)