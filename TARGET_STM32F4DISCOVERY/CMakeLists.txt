# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-stm32f4discovery INTERFACE)

target_sources(mbed-stm32f4discovery
    INTERFACE
        PeripheralPins.c
		system_clock.c
)

target_include_directories(mbed-stm32f4discovery
    INTERFACE
        .
)

target_link_libraries(mbed-stm32f4discovery INTERFACE mbed-stm32f407xg)
