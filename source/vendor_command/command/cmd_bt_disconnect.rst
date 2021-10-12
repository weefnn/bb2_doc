.. _CMD_BT_DISCONNECT_ref:

CMD_BT_DISCONNECT
#################

.. list-table:: **Command Format**
   :widths: 15 10 20 15
   :header-rows: 1

   * - Command
     - Command ID
     - Command Parameters
     - Return Event
   * - CMD_BT_DISCONNECT
     - 0x0003
     - bd_addr, flag
     - :ref:`EVENT_BT_DISCONNECT_STATUS_ref`

Description
***********

This command is used to cancel the ongoing link back procedure or disconnect the linked profiles. 
BTM will disconnect ACL link if all of the profiles is disconnected.

Command Parameters
******************

.. list-table:: **bd_addr** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX
     - MAC address with low byte first of the target device that wants to disconnect

.. list-table:: **flag : bitmask** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX
     - | bit0:A2DP_PROFILE_MSAK
       | bit1:AVRCP_PROFILE_MSAK
       | bit2:HFHS_PROFILE_MSAK
       | bit3:VENDOR_PROFILE_MSAK
       | bit4:SPP_PROFILE_MSAK
       | bit5:IAP_PROFILE_MSAK
       | bit6:PBAP_PROFILE_MSAK
       | bit7:reserved




