# Source: https://os.mbed.com/docs/mbed-os/v6.15/porting/porting-custom-boards.html

add_library(mbed-f405a INTERFACE)

target_sources(mbed-f405a
    INTERFACE
        PeripheralPins.c
		system_clock.c
)

target_include_directories(mbed-f405a
    INTERFACE
        .
)

target_link_libraries(mbed-f405a INTERFACE mbed-stm32f405xg)
