add_library(solver_lib solver_lib.cpp solver.cpp)
target_include_directories(solver_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
