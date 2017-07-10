---
title: WDI\_TLV\_WAKE\_PACKET\_BITMAP\_PATTERN
description: WDI\_TLV\_WAKE\_PACKET\_BITMAP\_PATTERN is a TLV that contains a wake-on-LAN pattern.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 5BE0F668-A3B4-4ECF-B963-EC4DD1B1A8AE
keywords: ["WDI_TLV_WAKE_PACKET_BITMAP_PATTERN Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_WAKE_PACKET_BITMAP_PATTERN
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_WAKE\_PACKET\_BITMAP\_PATTERN


WDI\_TLV\_WAKE\_PACKET\_BITMAP\_PATTERN is a TLV that contains a wake-on-LAN pattern.

## TLV Type


0x5B

## Length


The sum (in bytes) of the sizes of all contained TLVs.

## Values


| Type                                                                                         | Multiple TLV instances allowed | Optional | Description                                                                  |
|----------------------------------------------------------------------------------------------|--------------------------------|----------|------------------------------------------------------------------------------|
| [**WDI\_TLV\_WAKE\_PACKET\_BITMAP\_PATTERN\_ID**](wdi-tlv-wake-packet-bitmap-pattern-id.md) |                                |          | Specifies the wake-on-LAN pattern ID.                                        |
| [**WDI\_TLV\_BITMAP\_PATTERN**](wdi-tlv-bitmap-pattern.md)                                  |                                |          | Specifies the wake-on-LAN pattern.                                           |
| [**WDI\_TLV\_BITMAP\_PATTERN\_MASK**](wdi-tlv-bitmap-pattern-mask.md)                       |                                |          | Specifies the wake-on-LAN pattern mask. The length is (PatternLength + 7)/8. |

 

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

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_WAKE_PACKET_BITMAP_PATTERN%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")



