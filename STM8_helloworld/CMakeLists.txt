cmake_minimum_required(VERSION 3.5)

project ( stm8-sample-proj )

include_directories (
    STM8S_StdPeriph_Driver/inc
     .
     )

set(MCU stm8)
set(CMAKE_C_FLAGS "-m${MCU} -DSTM8S003 -V --opt-code-size --verbose")

add_executable ( stm8-sample
     main.c
     main.h
     stm8s_it.c
     stm8s_it.h
     stm8s_conf.h
     
    STM8S_StdPeriph_Driver/inc/stm8s_uart3.h
    STM8S_StdPeriph_Driver/inc/stm8s_wwdg.h
    STM8S_StdPeriph_Driver/inc/stm8s_uart1.h
    STM8S_StdPeriph_Driver/inc/stm8s_tim3.h
    STM8S_StdPeriph_Driver/inc/stm8s_beep.h
    STM8S_StdPeriph_Driver/inc/stm8s_exti.h
    STM8S_StdPeriph_Driver/inc/stm8s_rst.h
    STM8S_StdPeriph_Driver/inc/stm8s_iwdg.h
    STM8S_StdPeriph_Driver/inc/stm8s_awu.h
    STM8S_StdPeriph_Driver/inc/fireworks.h
    STM8S_StdPeriph_Driver/inc/stm8s_spi.h
    STM8S_StdPeriph_Driver/inc/stm8s_clk.h
    STM8S_StdPeriph_Driver/inc/stm8s_flash.h
    STM8S_StdPeriph_Driver/inc/stm8s.h
    STM8S_StdPeriph_Driver/inc/stm8s_gpio.h
    STM8S_StdPeriph_Driver/inc/stm8s_can.h
    STM8S_StdPeriph_Driver/inc/stm8s_tim6.h
    STM8S_StdPeriph_Driver/inc/stm8s_tim2.h
    STM8S_StdPeriph_Driver/inc/stm8s_tim4.h
    STM8S_StdPeriph_Driver/inc/stm8s_tim5.h
    STM8S_StdPeriph_Driver/inc/stm8s_uart4.h
    STM8S_StdPeriph_Driver/inc/stm8s_uart2.h
    STM8S_StdPeriph_Driver/inc/stm8s_adc1.h
    STM8S_StdPeriph_Driver/inc/stm8s_i2c.h
    STM8S_StdPeriph_Driver/inc/stm8s_adc2.h
    STM8S_StdPeriph_Driver/inc/stm8s_tim1.h
    STM8S_StdPeriph_Driver/inc/stm8s_itc.h
    STM8S_StdPeriph_Driver/src/stm8s_adc1.c
    STM8S_StdPeriph_Driver/src/stm8s_i2c.c
    STM8S_StdPeriph_Driver/src/stm8s_clk.c
    STM8S_StdPeriph_Driver/src/stm8s_rst.c
    STM8S_StdPeriph_Driver/src/stm8s_awu.c
    STM8S_StdPeriph_Driver/src/stm8s_tim2.c
#     STM8S_StdPeriph_Driver/src/stm8s_tim6.c
    STM8S_StdPeriph_Driver/src/stm8s_itc.c
#     STM8S_StdPeriph_Driver/src/stm8s_can.c
#     STM8S_StdPeriph_Driver/src/stm8s_tim3.c
#     STM8S_StdPeriph_Driver/src/stm8s_uart4.c
    STM8S_StdPeriph_Driver/src/stm8s_tim1.c
    STM8S_StdPeriph_Driver/src/stm8s_gpio.c
#     STM8S_StdPeriph_Driver/src/stm8s_adc2.c
#     STM8S_StdPeriph_Driver/src/stm8s_tim5.c
    STM8S_StdPeriph_Driver/src/stm8s_flash.c
    STM8S_StdPeriph_Driver/src/stm8s_tim4.c
    STM8S_StdPeriph_Driver/src/fireworks.c
    STM8S_StdPeriph_Driver/src/stm8s_exti.c
    STM8S_StdPeriph_Driver/src/stm8s_wwdg.c
#     STM8S_StdPeriph_Driver/src/stm8s_uart3.c
    STM8S_StdPeriph_Driver/src/stm8s_beep.c
    STM8S_StdPeriph_Driver/src/stm8s_iwdg.c
#     STM8S_StdPeriph_Driver/src/stm8s_uart2.c
    STM8S_StdPeriph_Driver/src/stm8s_spi.c
    STM8S_StdPeriph_Driver/src/stm8s_uart1.c
     )
