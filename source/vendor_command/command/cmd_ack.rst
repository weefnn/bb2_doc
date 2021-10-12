.. _CMD_ACK_ref:

CMD_ACK
#######

.. list-table:: **Command Format**
   :widths: 15 10 20 15
   :header-rows: 1

   * - Command
     - Command ID
     - Command Parameters
     - Return Event
   * - CMD_ACK
     - 0x0000
     - event_id, status
     - 

Description
***********

This command is used for MCU to ack the received BTM's EVENT.

Command Parameters
******************

.. list-table:: **event_id** SIZE: 2 BYTE
   :widths: 15 30
   :header-rows: 1

   * - 
     - Parameter Description
   * - 0xXX
     - the acked event_id

.. list-table:: **status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - command complete : MCU can handle this command.
   * - 0x01
     - command disallow : MCU can not handle this command.
   * - 0x02
     - unknow CMD
   * - 0x03
     - parameters error
   * - 0x04
     - busy
   * - 0x05
     - process fail
   * - 0x06
     - one wire extend
   * - others
     - one wire extend



