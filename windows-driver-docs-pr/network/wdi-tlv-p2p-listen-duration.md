---
title: WDI\_TLV\_P2P\_LISTEN\_DURATION
description: WDI\_TLV\_P2P\_LISTEN\_DURATION is a TLV that contains Wi-Fi Direct listen duration information.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 6C14BB67-89E1-4795-9327-2B5B87BF2D7C
keywords: ["WDI_TLV_P2P_LISTEN_DURATION Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_P2P_LISTEN_DURATION
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_P2P\_LISTEN\_DURATION


WDI\_TLV\_P2P\_LISTEN\_DURATION is a TLV that contains Wi-Fi Direct listen duration information.

## TLV Type


0xE9

## Length


The sum (in bytes) of the sizes of all contained elements.

## Values


| Type   | Description                                                                                                                                                    |
|--------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| UINT32 | The duration, in milliseconds, of the listen cycle. The adapter is in listen state during this time.                                                           |
| UINT32 | The duration, in milliseconds, that the adapter is expected to actively listen during the listen cycle. This duration must be less than listen cycle duration. |

 

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

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_P2P_LISTEN_DURATION%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




