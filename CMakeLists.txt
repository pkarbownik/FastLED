idf_component_register(SRCS FastLED.cpp		colorpalettes.cpp	hsv2rgb.cpp		noise.cpp		power_mgt.cpp
bitswap.cpp		colorutils.cpp		lib8tion.cpp		platforms.cpp		wiring.cpp esp32-hal.c esp32-hal-gpio.c
                       INCLUDE_DIRS "."
                       REQUIRES nvs_flash )
add_definitions(-DESP32)
target_compile_options(${COMPONENT_LIB} PRIVATE -Wno-error=class-memaccess)