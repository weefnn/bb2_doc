.. _EVENT_ACK_ref:

EVENT_ACK
#########

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_ACK
     - 0x0000
     - cmd_id, status

Description
***********

This event is used to ack the received command.

Event Parameters
****************

.. list-table:: **cmd_id** SIZE: 2 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX
     - the command id to ack

.. list-table:: **status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - command complete : BTM can handle this command.
   * - 0x01
     - command disallow : BTM can not handle this command.
   * - 0x02
     - unknow CMD
   * - 0x03
     - parameters error
   * - 0x04
     - busy
   * - 0x05
     - process fail: maybe due to stack resource
   * - others
     - RFD



