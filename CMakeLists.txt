cmake_minimum_required(VERSION 3.8)

# Edit the project name here
project(cuda_test)
set(CPACK_PACKAGE_DESCRIPTION_SUMMARY "CUDA test application")

# NLOpt
set(libs ${libs} nlopt)

# Armadillo
set(libs ${libs} armadillo)
set(libs ${libs} openblas)

# Call the standard device cmake build
include(/usr/local/share/cmake/so_cmake/application.cmake)
