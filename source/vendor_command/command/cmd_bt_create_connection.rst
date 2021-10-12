.. _CMD_BT_CREATE_CONNECTION_ref:

CMD_BT_CREATE_CONNECTION
########################

.. list-table:: **Command Format**
   :widths: 15 10 20 15
   :header-rows: 1

   * - Command
     - Command ID
     - Command Parameters
     - Return Event
   * - CMD_BT_CREATE_CONNECTION
     - 0x0002
     - profile, bd_addr
     - :ref:`EVENT_BT_CONNECT_STATUS`

Description
***********

This command is used to trigger the link back behavior for specific profiles.

Command Parameters
******************

.. list-table:: **profile(only for type = 0x04)** SIZE: 1 BYTE
   :widths: 15 50
   :header-rows: 1

   * - 
     - Parameter Description
   * - 0xXX
     - | bit mask:
       | bit0:A2DP
       | bit1:AVRCP
       | bit2:HF
       | bit3:Multi speaker
       | bit4:SPP
       | bit5:IAP
       | bit6:PBAP
       | bit7:HSF

.. list-table:: **bd_addr(only for type = 0x04)** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x..
     - MAC address of the dedicate device with low byte first




