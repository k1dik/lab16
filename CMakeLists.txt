cmake_minimum_required(VERSION 3.10)
project(solver_application)

add_subdirectory(solver_lib)
add_subdirectory(solver)

set(CPACK_GENERATOR "TGZ;ZIP;DEB;RPM")

set(CPACK_PACKAGE_NAME "solver")
set(CPACK_PACKAGE_VERSION "1.0.0")
set(CPACK_PACKAGE_CONTACT "youremail@example.com") # поменяй на свой email
set(CPACK_PACKAGE_DESCRIPTION_SUMMARY "Solver application for lab work")

# DEB package settings
set(CPACK_DEBIAN_PACKAGE_MAINTAINER "Your Name") # поменяй на своё имя
set(CPACK_DEBIAN_PACKAGE_DEPENDS "libc6 (>= 2.27)")

# RPM package settings
set(CPACK_RPM_PACKAGE_LICENSE "MIT")
set(CPACK_RPM_PACKAGE_GROUP "Applications/Engineering")
set(CPACK_RPM_PACKAGE_SUMMARY "Solver app")
set(CPACK_RPM_PACKAGE_DESCRIPTION "Solver application built using CMake for lab work")

include(CPack)
