cmake_minimum_required(VERSION 3.10)
project(solver_application)

add_subdirectory(solver_lib)
add_subdirectory(solver)

set(CPACK_GENERATOR "TGZ;ZIP;DEB;RPM")
set(CPACK_PACKAGE_NAME "solver")
set(CPACK_PACKAGE_VERSION "1.0.0")
set(CPACK_DEBIAN_PACKAGE_MAINTAINER "Your Name") # поменяй на свое имя если хочешь
include(CPack)
