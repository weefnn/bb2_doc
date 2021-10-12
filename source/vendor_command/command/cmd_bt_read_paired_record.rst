.. _CMD_BT_READ_PAIRED_RECORD_ref:


CMD_BT_READ_PAIRED_RECORD
#########################

.. list-table:: **Command Format**
   :widths: 15 10 20 15
   :header-rows: 1

   * - Command
     - Command ID
     - Command Parameters
     - Return Event
   * - CMD_BT_READ_PAIRED_RECORD
     - 0x0001
     - type
     - :ref:`EVENT_REPLY_PAIRED_RECORD_ref`

Description
***********

This command is used to read the paired device information of BTM recorded.

Command Parameters
******************

.. list-table:: **type** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - 
     - Parameter Description
   * - 0xXX
     - reserved
