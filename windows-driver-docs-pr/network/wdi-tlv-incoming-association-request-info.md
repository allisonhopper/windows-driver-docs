---
title: WDI\_TLV\_INCOMING\_ASSOCIATION\_REQUEST\_INFO
description: WDI\_TLV\_INCOMING\_ASSOCIATION\_REQUEST\_INFO is a TLV that contains information about the incoming association request.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: E36ADD95-1751-4FCE-9032-900968878DEE
keywords: ["WDI_TLV_INCOMING_ASSOCIATION_REQUEST_INFO Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_INCOMING_ASSOCIATION_REQUEST_INFO
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_INCOMING\_ASSOCIATION\_REQUEST\_INFO


WDI\_TLV\_INCOMING\_ASSOCIATION\_REQUEST\_INFO is a TLV that contains information about the incoming association request.

## TLV Type


0x8F

## Length


The sum (in bytes) of the sizes of all contained TLVs.

## Values


| Type                                                                                                            | Multiple TLV instances allowed | Optional | Description                                                      |
|-----------------------------------------------------------------------------------------------------------------|--------------------------------|----------|------------------------------------------------------------------|
| [**WDI\_TLV\_INCOMING\_ASSOCIATION\_REQUEST\_PARAMETERS**](wdi-tlv-incoming-association-request-parameters.md) |                                |          | The parameters for the incoming association request.             |
| [**WDI\_TLV\_ASSOCIATION\_REQUEST\_FRAME**](wdi-tlv-association-request-frame.md)                              |                                |          | The association request frame.                                   |
| [**WDI\_TLV\_ASSOCIATION\_REQUEST\_DEVICE\_CONTEXT**](wdi-tlv-association-request-device-context.md)           |                                | X        | The vendor-specific information that is passed down to the port. |

 

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

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_INCOMING_ASSOCIATION_REQUEST_INFO%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




