.. _event_reference:

EVENT
#####

summary of event.

.. list-table:: Event Table
   :widths: 15 30 10
   :header-rows: 1

   * - Command ID
     - Command
     - Available
   * - 0x0000
     - :ref:`EVENT_ACK_ref`
     - Y
   * - 0x0001
     - :ref:`EVENT_BT_REPLY_PAIRED_RECORD_ref`
     - Y
   * - 0x0003
     - :ref:`EVENT_BT_CONNECT_STATUS_ref`
     - Y
   * - 0x0004
     - :ref:`EVENT_BT_DISCONNECT_STATUS_ref`
     - Y
   * - 0x0007
     - :ref:`EVENT_AUDIO_DEVICE_STATE_ref`
     - Y
   * - 0x000A
     - :ref:`EVENT_AUDIO_CALL_STATUS_ref`
     - Y
   * - 0x000B
     - :ref:`EVENT_AUDIO_PLAYER_STATUS_ref`
     - N
   * - 0x0014
     - :ref:`EVENT_BT_LINK_STATUS_ref`
     - Y
   * - 0x0300
     - :ref:`EVENT_SCO_STATE_ref`
     - Y

.. toctree::
   :maxdepth: 1

   event_ack.rst
   event_bt_reply_paired_record.rst
   event_bt_connect_status.rst
   event_bt_disconnect_status.rst
   event_audio_device_state.rst
   event_audio_call_status.rst
   event_audio_player_status.rst
   event_bt_link_status.rst
   event_sco_state.rst