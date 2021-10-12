.. _EVENT_SCO_STATE_ref:

EVENT_SCO_STATE
###############

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_SCO_STATE
     - 0x0300
     - connect_status, address

Description
***********

This event is used to report SCO connect state

Event Parameters
****************

.. list-table:: **connect_status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - no sco
   * - 0x00
     - SCO link established

.. list-table:: **address** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX...
     - the remote device BT address


