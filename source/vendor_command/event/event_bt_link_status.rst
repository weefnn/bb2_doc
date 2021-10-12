.. _EVENT_BT_LINK_STATUS_ref:

EVENT_BT_LINK_STATUS
####################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_BT_LINK_STATUS
     - 0x0014
     - link_status, bd_addr

Description
***********

report link(ACL) status to MCU

Event Parameters
****************

.. list-table:: **link_status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - LINK_STATE_STANDBY
   * - 0x01
     - LINK_STATE_CONNECTED
   * - 0x02
     - LINK_STATE_LOST
   * - 0x03
     - LINK_STATE_CONN_FAIL

.. list-table:: **bd_addr** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX...
     - remote device address





