---
title: WDI\_TLV\_P2P\_WPS\_ENABLED
description: WDI\_TLV\_P2P\_WPS\_ENABLED is a TLV that specifies if Wi-Fi Protected Setup is enabled.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: B923DA17-451C-4BF1-8B8B-C2846EDE9774
keywords: ["WDI_TLV_P2P_WPS_ENABLED Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_P2P_WPS_ENABLED
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_P2P\_WPS\_ENABLED


WDI\_TLV\_P2P\_WPS\_ENABLED is a TLV that specifies if Wi-Fi Protected Setup is enabled.

## TLV Type


0xF7

## Length


The size (in bytes) of a UINT8.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Type</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>UINT8</td>
<td>Specifies if Wi-Fi Protected Setup is enabled.
<p>Valid values are 0 (not enabled) and 1 (enabled).</p></td>
</tr>
</tbody>
</table>

 

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


[OID\_WDI\_SET\_P2P\_WPS\_ENABLED](https://msdn.microsoft.com/library/windows/hardware/dn925938)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_P2P_WPS_ENABLED%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





