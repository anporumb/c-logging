#Copyright (c) Microsoft. All rights reserved.
#Licensed under the MIT license. See LICENSE file in the project root for full license information.

cmake_minimum_required(VERSION 2.8.11)

#unit tests
if(${run_unittests})
    if(WIN32)
       add_subdirectory(logging_ut)
    endif()
endif()

if(${run_int_tests})
    if(WIN32)
       add_subdirectory(logging_int)
    endif()
endif()
