---
title: WDI\_TLV\_P2P\_PROVISION\_DISCOVERY\_RESPONSE\_INFO
description: WDI\_TLV\_P2P\_PROVISION\_DISCOVERY\_RESPONSE\_INFO is a TLV that contains Wi-Fi Direct Provision Discovery Response information.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: EB7C4A5C-27D8-4A84-BC91-0DED51FB74C2
keywords: ["WDI_TLV_P2P_PROVISION_DISCOVERY_RESPONSE_INFO Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_P2P_PROVISION_DISCOVERY_RESPONSE_INFO
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_P2P\_PROVISION\_DISCOVERY\_RESPONSE\_INFO


WDI\_TLV\_P2P\_PROVISION\_DISCOVERY\_RESPONSE\_INFO is a TLV that contains Wi-Fi Direct Provision Discovery Response information.

## TLV Type


0x87

## Length


The sum (in bytes) of the sizes of all contained TLVs.

## Values


| Type                                                                                                                     | Multiple TLV instances allowed | Optional | Description                                                                                                                                                                                                                             |
|--------------------------------------------------------------------------------------------------------------------------|--------------------------------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**WDI\_TLV\_P2P\_PROVISION\_DISCOVERY\_RESPONSE\_PARAMETERS**](wdi-tlv-p2p-provision-discovery-response-parameters.md) |                                |          | The provision discovery response parameters.                                                                                                                                                                                            |
| [**WDI\_TLV\_P2P\_PROVISION\_SERVICE\_ATTRIBUTES**](wdi-tlv-p2p-provision-service-attributes.md)                        |                                | X        | The Provision Service attributes.                                                                                                                                                                                                       |
| [**WDI\_TLV\_P2P\_GROUP\_ID**](wdi-tlv-p2p-group-id.md)                                                                 |                                | X        | The Group ID if Wi-Fi Direct Service is supported.                                                                                                                                                                                      |
| [**WDI\_TLV\_P2P\_PERSISTENT\_GROUP\_ID**](wdi-tlv-p2p-persistent-group-id.md)                                          |                                | X        | The Group IP for the Persistent Group to be used for the connection. This field is valid if the Persistent Group flag in [**WDI\_TLV\_P2P\_PROVISION\_SERVICE\_ATTRIBUTES**](wdi-tlv-p2p-provision-service-attributes.md) is set to 1. |
| [**WDI\_TLV\_P2P\_SERVICE\_SESSION\_INFO**](wdi-tlv-p2p-service-session-info.md)                                        |                                | X        | The Service Session information.                                                                                                                                                                                                        |

 

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum supported client</p></td>
<td><p>Windows 10</p></td>
</tr>
<tr class="even">
<td><p>Minimum supported server</p></td>
<td><p>Windows Server 2016</p></td>
</tr>
<tr class="odd">
<td><p>Header</p></td>
<td>Wditypes.hpp</td>
</tr>
</tbody>
</table>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_P2P_PROVISION_DISCOVERY_RESPONSE_INFO%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




