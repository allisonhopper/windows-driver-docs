---
title: WDI\_TLV\_CIPHER\_KEY\_BIP\_KEY
description: WDI\_TLV\_CIPHER\_KEY\_BIP\_KEY is a TLV that contains BIP cipher algorithm key data for OID\_WDI\_SET\_ADD\_CIPHER\_KEYS.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 99630BDF-9845-4E3D-AB18-5F5BAFCF7198
keywords: ["WDI_TLV_CIPHER_KEY_BIP_KEY Network Drivers Starting with Windows Vista"]
topic_type:
- apiref
api_name:
- WDI_TLV_CIPHER_KEY_BIP_KEY
api_location:
- wditypes.hpp
api_type:
- HeaderDef
---

# WDI\_TLV\_CIPHER\_KEY\_BIP\_KEY


WDI\_TLV\_CIPHER\_KEY\_BIP\_KEY is a TLV that contains BIP cipher algorithm key data for [OID\_WDI\_SET\_ADD\_CIPHER\_KEYS](https://msdn.microsoft.com/library/windows/hardware/dn925855).

## TLV Type


0x51

## Length


The size (in bytes) of the array of UINT8 elements. The array must contain 1 or more elements.

## Values


| Type      | Description                              |
|-----------|------------------------------------------|
| UINT8\[\] | Specifies BIP cipher algorithm key data. |

 

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

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bnetvista\netvista%5D:%20WDI_TLV_CIPHER_KEY_BIP_KEY%20%20RELEASE:%20%287/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




