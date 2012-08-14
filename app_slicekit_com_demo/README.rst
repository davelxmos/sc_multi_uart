Multi Uart Slicekit Demo
========================

:scope: Example
:description: An example application that demonstrates the multi-uart
              component on a slicekit board
:keywords: uart, slicekit

This application serves as a sample demonstration on how to utilize
MultiUART component. It uses the module_multi_uart and module_xc_ptr modules.


To use this demo, first edit the main.xc source file and change the 
slice kit slot as per your hardware configuration usage:

[SLICE KIT MACRO] - TBA

Now build the project and connect the MUART slice . You should
be able to open HyperTerminal or any terminal client software and key in 
any data and help appears on the screen.

Key Source Files:

    main.xc : top-level file showing what threads are running

    uart_manager.xc : multi-UART application handler managing UART data from 
              transmit and receive threads  
