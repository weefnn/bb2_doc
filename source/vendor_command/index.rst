.. _vendor_command_reference:

Vendor Command
##############

This is an introduction of UART transfer packet format.

+--------------+------------+-------+---------------------------+---------------------------+------------+------------+
|              | SINC WORD  | Seqn  | LENGTH                    | cmd/event op code         | parameters | CHK SUM    |
+==============+============+=======+===========================+===========================+============+============+
| BYTE NO      | 0          | 1     | 2(low byte) ,3(high byte) | 4(low byte) ,5(high byte) | 6 ~        | LENGTH + 4 |
+--------------+------------+-------+---------------------------+---------------------------+------------+------------+
| SIZE (BYTES) | 1          | 1     |             2             |             2             | LENGTH - 2 | 1          |
+--------------+------------+-------+---------------------------+---------------------------+------------+------------+
| VALUE        | 0xAA       | 1~255 |           1～65535        | cmd/event                 | DATA       | CHK SUM    |
+--------------+------------+-------+---------------------------+---------------------------+------------+------------+
|                           | Check sum to be calculated                                                 |            |
+---------------------------+-----------------------------------+----------------------------------------+------------+
|                                                               | LENGTH                                 |            |
+---------------------------------------------------------------+----------------------------------------+------------+


**LENGTH**: Data length includes cmd/event op code and parameters	

**Check SUM Rule** : Summation from Seq to CHK SUM is 0x00, this field only valid for uart path 

**Example** : tone gen command		

for uart path : AA 01 04 00 08 00 01 00 F2	

.. toctree::
    :maxdepth: 1
    :caption: Command & Event

    command/index.rst
    event/index.rst

