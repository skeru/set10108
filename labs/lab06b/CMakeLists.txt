project(set10108-lab06b LANGUAGES CXX CUDA)
cmake_minimum_required(VERSION 3.17)
set(CMAKE_CXX_STANDARD 17)
include_directories(../contrib)
 
add_executable(smooth-2d smooth-2d.cu)
set_property(TARGET smooth-2d PROPERTY CUDA_SEPARABLE_COMPILATION ON)