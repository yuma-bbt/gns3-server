/v2/compute/projects/{project_id}/cloud/nodes/{node_id}/adapters/{adapter_number:\d+}/ports/{port_number:\d+}/start_capture
------------------------------------------------------------------------------------------------------------------------------------------

.. contents::

POST /v2/compute/projects/**{project_id}**/cloud/nodes/**{node_id}**/adapters/**{adapter_number:\d+}**/ports/**{port_number:\d+}**/start_capture
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Start a packet capture on a cloud instance

Parameters
**********
- **adapter_number**: Adapter on the cloud (always 0)
- **node_id**: Node UUID
- **port_number**: Port on the cloud
- **project_id**: Project UUID

Response status codes
**********************
- **200**: Capture started
- **400**: Invalid request
- **404**: Instance doesn't exist

Input
*******
.. raw:: html

    <table>
    <tr>                 <th>Name</th>                 <th>Mandatory</th>                 <th>Type</th>                 <th>Description</th>                 </tr>
    <tr><td>capture_file_name</td>                    <td>&#10004;</td>                     <td>string</td>                     <td>Capture file name</td>                     </tr>
    <tr><td>data_link_type</td>                    <td> </td>                     <td>enum</td>                     <td>Possible values: DLT_ATM_RFC1483, DLT_EN10MB, DLT_FRELAY, DLT_C_HDLC</td>                     </tr>
    </table>
