cmake_minimum_required(VERSION 2.8)

include(../config/copy_utils.cmake)

project(test_suite)

copydir(HardwareFaults HardwareFaults)
copydir(SoftwareFaults SoftwareFaults)
copydir(PROGRAMS PROGRAMS)
copydir(Traces Traces)
copydir(BatchMode BatchMode)
copydir(MakefileGeneration MakefileGeneration)
copy(test_suite.yaml test_suite.yaml)

add_subdirectory(SCRIPTS)

genCopy()

