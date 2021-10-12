.. _EVENT_BT_CONNECT_STATUS_ref:

EVENT_BT_CONNECT_STATUS
#######################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_BT_CONNECT_STATUS
     - 0x0003
     - connect_status, address

Description
***********

This event is used to report current bt profiles connect status

Event Parameters
****************

.. list-table:: **connect_status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - reserved
   * - 0x01
     - A2DP_PROFILE_MSAK   
   * - 0x02
     - AVRCP_PROFILE_MSAK
   * - 0x04
     - HFHS_PROFILE_MSAK
   * - 0x08
     - VENDOR_PROFILE_MSAK
   * - 0x10
     - SPP_PROFILE_MSAK
   * - 0x20
     - IAP_PROFILE_MSAK
   * - 0x40
     - PBAP_PROFILE_MSAK
   * - 0x80
     - HSP_PROFILE_MSAK

.. list-table:: **address** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX...
     - the remote device BT address


