Introduction
==============

The Multi-UART component provides a software library that allows the use of 8 bit ports for multiple channel UART communication. This library is dynamically re-configurable for applications that require a level of flexibility during operation.

This document describes an overview of the Multi-UART component, resource requirements, API and programming details. It follows the examples that are given in the app_multi_uart_demo.

Supported Functionality
------------------------

The Multi-UART provides the following functionality. All options are dynamically reconfigurable via the API.

.. list-table::
    :header-rows: 1
    
    * - Function
      - Operational Range
      - Notes
    * - Baud Rate
      - 150 to 115200 bps
      - Dependent on clocking (see :ref:`sec_ext_clk`)
    * - Parity
      - {None, Mark, Space, Odd, Even}
      - 
    * - Stop Bits
      - {1,2}
      -
    * - Data Length
      - 1 to 30 bits
      - Max 30 bits assumes 1 stop bit and no parity.

Slicekit Compatibility
----------------------

SliceKit logo [TBA]

MUART slice is an I/O slice and is compatible to all connectors of the Slicekit Core board.

.. _fig_slicekit_compatibility:

.. figure:: images/all_slots_compatible.png
    :align: center
    :width: 50%
    
    Slicekit Core board connector compatibilty
