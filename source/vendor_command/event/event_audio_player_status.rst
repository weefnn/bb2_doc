.. _EVENT_AUDIO_PLAYER_STATUS_ref:

EVENT_AUDIO_PLAYER_STATUS
#########################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_ACK
     - 0x000B
     - bd_addr, status, codec_type

Description
***********

This event is used to report current play status.

Event Parameters
****************

.. list-table:: **bd_addr** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX
     - MAC address of the remote connected device whose play status has changed.

.. list-table:: **status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - STOP
   * - 0x01
     - PLAYING
   * - 0x02
     - PAUSED
   * - 0x03
     - FWD_SEEK
   * - 0x04
     - REV_SEEK
   * - 0x05
     - REV_SEEK
   * - 0x06
     - REWIND
   * - others
     - RFD

.. list-table:: **codec_type** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - SBC Streaming
   * - 0x02
     - AAC Streaming

