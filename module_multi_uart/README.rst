Multi Uart Module
=================

:scope: General Use
:description: A module capable of implementing up to 8 uarts (rx and tx) on a single logical core
:keywords: uart

This module provides the capability to run a task on a single logical
core that implements up to 8 uart recievers and 8 uart transmitters.

The Multi-UART provides the following functionality. All options are dynamically reconfigurable via the API.

.. list-table::
    :header-rows: 1
    
    * - Function
      - Operational Range
    * - Baud Rate
      - 150 to 115200 bps
    * - Parity
      - {None, Mark, Space, Odd, Even}
    * - Stop Bits
      - {1,2}
    * - Data Length
      - 1 to 30 bits

Full details of how the module is used can be found in the module
design guide.
