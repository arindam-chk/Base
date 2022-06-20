project(Base)
cmake_minimum_required(VERSION 3.0)
enable_testing()


#####################################################################################
include(ExternalProject)
ExternalProject_Add(Cogent
    SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/modules/Cogent
    PREFIX ${CMAKE_CURRENT_SOURCE_DIR}/Cogent
    INSTALL_COMMAND ""
    )

ExternalProject_Get_Property(Cogent source_dir binary_dir)
#####################################################################################


#####################################################################################
include(ExternalProject)
ExternalProject_Add(Yolox
    SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/modules/Yolox
    PREFIX ${CMAKE_CURRENT_SOURCE_DIR}/Yolox
    INSTALL_COMMAND ""
    )

ExternalProject_Get_Property(Yolox source_dir binary_dir)
#####################################################################################
