.. _EVENT_AUDIO_CALL_STATUS_ref:

EVENT_AUDIO_CALL_STATUS
########################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_AUDIO_CALL_STATUS
     - 0x000A
     - bd_addr, prev_status, curr_status

Description
***********

the call status of the connected device

Event Parameters
****************

.. list-table:: **bd_addr** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX...
     - MAC address of the remote connected device whose call status has changed.

.. list-table:: **prev_status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - CALL_IDLE
   * - 0x01
     - VOICE_ACTIVATION_ONGOING
   * - 0x02
     - INCOMING_CALL_ONGOING
   * - 0x03
     - OUTGOING_CALL_ONGOING
   * - 0x04
     - CALL_ACTIVE
   * - 0x05
     - CALL_ACTIVE_WITH_CALL_WAITING
   * - 0x06
     - CALL_ACTIVE_WITH_CALL_HOLD
   * - others
     - reserved

.. list-table:: **curr_status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - CALL_IDLE
   * - 0x01
     - VOICE_ACTIVATION_ONGOING
   * - 0x02
     - INCOMING_CALL_ONGOING
   * - 0x03
     - OUTGOING_CALL_ONGOING
   * - 0x04
     - CALL_ACTIVE
   * - 0x05
     - CALL_ACTIVE_WITH_CALL_WAITING
   * - 0x06
     - CALL_ACTIVE_WITH_CALL_HOLD
   * - others
     - reserved


