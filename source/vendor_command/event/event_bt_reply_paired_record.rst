.. _EVENT_BT_REPLY_PAIRED_RECORD_ref:

EVENT_BT_REPLY_PAIRED_RECORD
#############################

.. list-table:: **Event Format**
   :widths: 15 10 20
   :header-rows: 1

   * - Event
     - Event ID
     - Command Parameters
   * - EVENT_BT_REPLY_PAIRED_RECORD
     - 0x0001
     - paired_device_number, paired_record

Description
***********

This event is used to reply the  Read_Paired_Device_Information command.

Event Parameters
****************

.. list-table:: **paired_device_number** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - 0xXX
     - paired_device_number

.. list-table:: **paired_record** SIZE: (8*total_record) BYTE
   :widths: 15 30
   :header-rows: 1

   * - Value
     - Parameter Description
   * - byte0
     - link priority : 1 is the highest(newest device) and 4(or 8) is the lowest(oldest device)
   * - byte1
     - | bond_flag:
       | bit0:hf or hs profile_bond
       | bit1:a2dp profile bond
       | bit2:spp or iap profile bond
       | bit3:reserved for pbap
       | bit4:remote device support content protection
       | bit5:remote device support delay report
       | bit6:link key type is authenticated type
       | bit7:reserved
   * - byte2~byte7
     - linked device BD address (6 bytes with low byte first)

