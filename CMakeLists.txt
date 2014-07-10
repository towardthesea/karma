# Copyright: (C) 2012 Department of Robotics Brain and Cognitive Sciences - Istituto Italiano di Tecnologia
# Authors: Ugo Pattacini, Vadim Tikhanoff
# CopyPolicy: Released under the terms of the GNU GPL v2.0.

cmake_minimum_required(VERSION 2.6)
project(karma)

find_package(ICUBcontrib)
list(APPEND CMAKE_MODULE_PATH ${ICUBCONTRIB_MODULE_PATH})
include(ICUBcontribHelpers)

add_subdirectory(karmaManager)
add_subdirectory(karmaMotor)
add_subdirectory(karmaLearn)
add_subdirectory(karmaToolProjection)
add_subdirectory(karmaToolFinder)
add_subdirectory(app)

icubcontrib_add_uninstall_target()

