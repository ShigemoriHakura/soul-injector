idf_component_register(
        SRCS
            "main.cpp"
            "prog/swd_prog.cpp" "prog/includes/swd_prog.hpp"
            "prog/config_manager.cpp" "prog/includes/config_manager.hpp"
            "prog/swd_headless_flasher.cpp" "prog/includes/swd_headless_flasher.hpp"
            "external/includes/ArduinoJson.hpp" "prog/includes/led_ctrl.hpp"
            "misc/includes/file_utils.hpp"
            "comm/usb/cdc_acm.cpp" "comm/usb/includes/cdc_acm.hpp"
            "misc/includes/soul_nvs.hpp"
            "driver/includes/button_monitor.hpp"
            "driver/lcd/lhs154kc.c" "driver/lcd/lhs154kc.h"
            "driver/lcd/lvgl_wrapper.c" "driver/lcd/lvgl_wrapper.h"
            "driver/lcd/lcd_manager.cpp" "driver/lcd/lcd_manager.hpp"

        INCLUDE_DIRS
            "." "misc/includes" "prog/includes" "external/includes" "comm/usb/includes" "driver/includes" "driver"
        PRIV_REQUIRES
            "daplink-esp"
            "mbedtls"
            "spiffs"
            "usb"
            "spi_flash"
            "efuse"
            "nvs_flash"
            "driver"
            "esp_timer"
            "lvgl"
            "led_strip"
)
