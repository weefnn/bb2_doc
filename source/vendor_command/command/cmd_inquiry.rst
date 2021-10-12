.. _CMD_INQUIRY_ref:

CMD_INQUIRY
###########

.. list-table:: **Command Format**
   :widths: 15 10 20 15
   :header-rows: 1

   * - Command
     - Command ID
     - Command Parameters
     - Return Event
   * - CMD_INQUIRY
     - 0x0321
     - Action, TimeOut
     - :ref:`EVENT_INQUIRY_STATE`

Description
***********

This request search the neighbor Bluetooth devices

Command Parameters
******************

.. list-table:: **Action** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - 
     - Parameter Description
   * - 0x00
     - Start inquiry
   * - 0x01
     - stop inquiry 

.. list-table:: **TimeOut** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x01 ~ 0x30
     - | Maximum amount of time before the inquiry is halted.
       | Time = N * 1.28 sec.
       | Range : 1.28 – 61.44 sec







