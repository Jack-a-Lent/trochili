/*!
    \file  readme.txt
    \brief description of the TIMER2 input capture demo
*/

/*
    Copyright (C) 2016 GigaDevice

    2014-12-26, V1.0.0, firmware for GD32F1x0(x=3,5)
    2016-01-15, V2.0.0, firmware for GD32F1x0(x=3,5,7,9)
    2016-04-30, V3.0.0, firmware update for GD32F1x0(x=3,5,7,9)
*/

  This demo is based on the GD32150R-EVAL/GD32190R-EVAL board, it shows TIMER 
peripheral to measure the frequency of an external signal.
  
  The TIMxCLK frequency is set to systemcoreclock 72MHz,the prescaler is 36000 so 
the TIMER2 counter clock is 2KHz.
  
  The external signal is connected to TIMER2 CH0 pin (PB4).
  The rising edge is used as active edge.
  The TIMER2 CH0CV is used to compute the frequency value.

  The available frequence of the input signal is ranging from 0.03Hz to 2KHz.
You can use USART to watch the frequency of the input signal.The USART is
configured as follow:
  - BaudRate    = 115200 baud
  - Word Length = 8 Bits
  - One Stop Bit
  - No parity
  - Hardware flow control disabled (RTS and CTS signals)
  - Receive and transmit enabled
