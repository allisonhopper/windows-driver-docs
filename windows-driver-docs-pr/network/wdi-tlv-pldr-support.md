---
title: WDI\_TLV\_PLDR\_SUPPORT
description: WDI\_TLV\_PLDR\_SUPPORT is a TLV that specifies if PLDR (Platform Level Reset) is supported.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: BC1BE1A7-AA2D-4D11-A75A-EC0143343F33
keywords: ["WDI_TLV_PLDR_SUPPORT Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_PLDR_SUPPORT
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_PLDR\_SUPPORT


WDI\_TLV\_PLDR\_SUPPORT is a TLV that specifies if PLDR (Platform Level Reset) is supported.

**Note**  This TLV was added in Windows 10, version 1511, WDI version 1.0.10.

 

## TLV Type


0x11A

## Length


The size (in bytes) of a UINT8.

## Values


| Type  | Description                                                                                                                                                                                                                       |
|-------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| UINT8 | Specifies if PLDR is supported. This value is set to 0 if the device or bus does not support reset functionality (usually by querying the ACPI or PCI methods). A non-zero value specifies that reset functionality is supported. |

 

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

## See also


[PLDR](https://msdn.microsoft.com/library/windows/hardware/mt269098)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_PLDR_SUPPORT%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





