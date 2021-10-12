.. _CMD_MMI_ref:

CMD_MMI
#######

.. list-table:: **Command Format**
   :widths: 15 10 20 15
   :header-rows: 1

   * - Command
     - Command ID
     - Command Parameters
     - Return Event
   * - CMD_MMI
     - 0x0004
     - reserved, action
     - 

Description
***********

MMI action 

Command Parameters
******************

.. list-table:: **reserved** SIZE: 1 BYTE
   :widths: 15 30
   :header-rows: 1

   * - 
     - Parameter Description
   * - 0xXX
     - reserved

.. list-table:: **action description** SIZE: 1 BYTE
   :widths: 15 30 30
   :header-rows: 1

   * - Value
     - Parameter Description
     - Return Event
   * - 0x00
     - AU_MMI_NULL
     - 
   * - 0x03
     - AU_MMI_ANSWER_CALL: answer incoming call
     - :ref:`EVENT_AUDIO_CALL_STATUS_ref`
   * - 0x04
     - AU_MMI_REJECT_CALL: reject incoming call
     - :ref:`EVENT_AUDIO_CALL_STATUS_ref`
   * - 0x06
     - AU_MMI_DEV_MIC_MUTE_TOGGLE:mute mic if mic is ON, otherwise unmute mic
     - 
   * - 0x07
     - AU_MMI_DEV_MIC_MUTE:mute mic
     -
   * - 0x0B
     - AU_MMI_LAST_NUMBER_REDIAL:dail last number
     - :ref:`EVENT_AUDIO_CALL_STATUS_ref`
   * - 0x0D
     - AU_MMI_TRANSFER_TO_PHONE:when call active, add sco if sco doesn't exist, otherwise remove sco
     - 
   * - 0x15
     - MMI_DEV_MIC_VOL_UP:mic volume up
     - 
   * - 0x16
     - MMI_DEV_MIC_VOL_DOWN:mic volume down
     -
   * - 0x30
     - AU_MMI_DEV_SPK_VOL_UP
     - :ref:`EVENT_AUDIO_VOL_CHANGE_ref`
   * - 0x31
     - AU_MMI_DEV_SPK_VOL_DOWN
     - :ref:`EVENT_AUDIO_VOL_CHANGE_ref`
   * - 0x32
     - AU_MMI_AV_PLAY_PAUSE
     - :ref:`EVENT_AUDIO_PLAYER_STATUS_ref`
   * - 0x33
     - AU_MMI_AV_STOP
     - :ref:`EVENT_AUDIO_PLAYER_STATUS_ref`
   * - 0x51
     - AU_MMI_DEV_ENTER_PAIRING_MODE
     - :ref:`EVENT_AUDIO_DEVICE_STATE_ref`
   * - 0x52
     - AU_MMI_DEV_EXIT_PAIRING_MODE
     - 
   * - 0x53
     - AU_MMI_DEV_LINK_LAST_DEVICE
     - 
   * - 0x54
     - AU_MMI_DEV_POWER_ON_BUTTON_PRESS
     - :ref:`EVENT_AUDIO_DEVICE_STATE_ref`
   * - 0x56
     - AU_MMI_DEV_POWER_OFF_BUTTON_PRESS
     - :ref:`EVENT_AUDIO_DEVICE_STATE_ref`
   * - 0x58
     - AU_MMI_DEV_FACTORY_RESET_TO_DEFAULT
     - :ref:`EVENT_AUDIO_DEVICE_STATE_ref`
