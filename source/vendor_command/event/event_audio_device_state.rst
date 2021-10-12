.. _EVENT_AUDIO_DEVICE_STATE_ref:

EVENT_AUDIO_DEVICE_STATE
########################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_AUDIO_DEVICE_STATE
     - 0x0007
     - state, soc_legacy_addr

Description
***********

This event is used to report device state.

Event Parameters
****************

.. list-table:: **state** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - APP_STATE_OFF
   * - 0x01
     - APP_STATE_PAIRING
   * - 0x02
     - APP_STATE_STANDBY
   * - 0x03
     - APP_STATE_CONNECTED
   * - 0x04
     - AU_APP_STANDBY_WITH_LINK_BACK
   * - 0x05
     - AU_APP_CONNECTED_WITH_LINK_BACK
   * - others
     - reserved

.. list-table:: **soc_legacy_addr** SIZE: 6 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX...
     - the soc legacy BT address


