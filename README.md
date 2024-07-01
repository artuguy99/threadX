# threadX on stm32f407zet6
Hardware:

    PF8   --------> Led red
    PF9   --------> Led green
    PF10  --------> Led blue

    PH0   --------> Cristal oscillator 8M
    PH1   --------> Cristal oscillator 8M

    PA9   --------> USART1_TX
    PA10  --------> USART1_RX  Asynchronous 115200, 8, None, 1

    NRST  --------> Reset

Command:

    ~/stm32/threadX$ make
    ~/stm32/threadX$ openocd -f interface/stlink.cfg -f target/stm32f4x.cfg -c "program /home/artuguy/stm32/threadX/build/threadX.elf reset exit"

USART 1 Output：

Good afternoon
systemcoreclk = 168000000
thread 0 is running ... 
thread 0 is running ... 
thread 1 is running ... 
thread 0 is running ... 
thread 1 is running ... 

