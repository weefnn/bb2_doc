.. _EVENT_INQUIRY_STATE_ref:

EVENT_INQUIRY_STATE
###################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_INQUIRY_STATE
     - 0x0923
     - cmd_id, status

Description
***********

This event is used to report inquiry state.

Event Parameters
****************

.. list-table:: **state** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0x00
     - inquiry process has completed
   * - 0x01
     - inquiry process has cancelled
   * - 0x02
     - inquiry process contains a valid inquiry result
   * - 0x03
     - inquiry process fail


