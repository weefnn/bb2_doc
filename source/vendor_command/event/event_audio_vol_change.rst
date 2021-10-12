.. _EVENT_AUDIO_VOL_CHANGE_ref:

EVENT_AUDIO_VOL_CHANGE
######################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_AUDIO_VOL_CHANGE
     - 0x0020
     - status

Description
***********

report volume change information to remote device.

Event Parameters
****************

.. list-table:: **status** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - VolChangeNone
   * - 0x01
     - VolChangeUp
   * - 0x02
     - VolChangeDown
   * - 0x03
     - VolChangeMax
   * - 0x04
     - VolChangeMin


