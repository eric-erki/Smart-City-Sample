set(service "docker_swarm")
include("${CMAKE_SOURCE_DIR}/script/service.cmake")
include("${CMAKE_SOURCE_DIR}/script/deployment.cmake")
set_property(DIRECTORY APPEND PROPERTY ADDITIONAL_MAKE_CLEAN_FILES "${CMAKE_CURRENT_SOURCE_DIR}/docker-compose.yml")

if (NOT PLATFORM STREQUAL "VCAC-A")
    set(service "docker_compose")
    include("${CMAKE_SOURCE_DIR}/script/service.cmake")
    include("${CMAKE_SOURCE_DIR}/script/deployment.cmake")
endif()
