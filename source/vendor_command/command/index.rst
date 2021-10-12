.. _command_reference:

COMMAND
#######

summary of command.

.. list-table:: Command Table
   :widths: 15 30 10
   :header-rows: 1

   * - Command ID
     - Command
     - Available
   * - 0x0000
     - :ref:`CMD_ACK_ref`
     - Y
   * - 0x0001
     - :ref:`CMD_BT_READ_PAIRED_RECORD_ref`
     - Y
   * - 0x0002
     - :ref:`CMD_BT_CREATE_CONNECTION_ref`
     - Y
   * - 0x0003
     - :ref:`CMD_BT_DISCONNECT_ref`
     - Y
   * - 0x0004
     - :ref:`CMD_MMI_ref`
     - Y
   * - 0x0321
     - :ref:`CMD_INQUIRY_ref`
     - Y

.. toctree::
   :maxdepth: 1

   cmd_ack.rst
   cmd_bt_read_paired_record.rst
   cmd_bt_create_connection.rst
   cmd_bt_disconnect.rst
   cmd_mmi.rst
   cmd_inquiry.rst