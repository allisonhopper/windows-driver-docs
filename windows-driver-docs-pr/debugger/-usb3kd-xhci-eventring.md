---
title: usb3kd.xhci\_eventring
description: The usb3kd.xhci\_eventring extension displays information about the event ring data structure associated with a USB 3.0 host controller.
ms.assetid: D3A40372-5473-48B0-94C7-5D3B80801F16
keywords: ["usb3kd.xhci_eventring Windows Debugging"]
ms.author: windowsdriverdev
ms.date: 05/23/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
topic_type:
- apiref
api_name:
- usb3kd.xhci_eventring
api_type:
- NA
---

# !usb3kd.xhci\_eventring


The [**!usb3kd.xhci\_eventring**](-usb3kd-device-info.md) extension displays information about the event ring data structure associated with a USB 3.0 host controller.

```
!usb3kd.xhci_eventring DeviceExtension
```

## <span id="ddk__devobj_dbg"></span><span id="DDK__DEVOBJ_DBG"></span>Parameters


<span id="_______DeviceExtension______"></span><span id="_______deviceextension______"></span><span id="_______DEVICEEXTENSION______"></span> *DeviceExtension*   
Address of the device extension for the host controller's functional device object (FDO).

## <span id="DLL"></span><span id="dll"></span>DLL


Usb3kd.dll

Remarks
-------

The output **!xhci\_eventring** command is based on the data structures maintained by the USB 3.0 host controller driver (UsbXhci.sys). For more information about the USB 3.0 host controller driver and other drivers in the USB stack, see [USB Driver Stack Architecture](http://go.microsoft.com/fwlink/p?LinkID=251983).

The event ring is a structure used by the USB 3.0 host controller to inform drivers that an action has completed.

Examples
--------

To obtain the address of the device extension, look at the output of the [**!xhci\_dumpall**](-usb3kd-xhci-dumpall.md) command. In the following example, the address of the device extension is 0xfffffa800536e2d0.

```
3: kd> !xhci_dumpall

## Dumping all the XHCI controllers - DrvObj 0xfffffa80053072f0
------------------------------------------------------------
1)  ... - PCI: VendorId ... DeviceId ... RevisionId ... Firmware ...

    dt USBXHCI!_CONTROLLER_DATA 0xfffffa80052f20c0
    !rcdrlogdump USBXHCI -a 0xfffffa8005068520
    !rcdrlogdump USBXHCI -a 0xfffffa8004e8b9a0 (rundown)
    !wdfdevice 0x57ffac91fd8
    !xhci_capability 0xfffffa800536e2d0
    !xhci_registers 0xfffffa800536e2d0
    !xhci_commandring 0xfffffa800536e2d0 (No commands are pending)
    !xhci_deviceslots 0xfffffa800536e2d0
    !xhci_eventring 0xfffffa800536e2d0
    ...
```

Now you can pass the address of the device extension to the **!xhci\_eventring** command.

```
3: kd> !xhci_eventring 0xfffffa800536e2d0

## Dumping dt _PRIMARY_INTERRUPTER_DATA fffffa800536b5b0
-----------------------------------------------------

## [0] Interrupter : dt _INTERRUPTER_DATA 0xfffffa800536b7d0  !rcdrlogdump USBXHCI -a 0xfffffa8005aeab60
------------------------------------------------------------------------------------------------------
    DequeueSegment: 1 DequeueIndex: 217 TotalEventRingSegments: 2 TRBsPerSegment: 256
    CurrentBufferData : VA 0xfffffa8005373000 LA 0x117173000 !wdfcommonbuffer 0x57ffa65b9b8 Size 4096
    EventRingTableBufferData : VA 0xfffffa8005aeb000 LA 0x1168eb000 !wdfcommonbuffer 0x57ffa65d988 Size 512

    [0] VA 0xfffffa8005370000 LA 0x117170000 !wdfcommonbuffer 0x57ffa6599b8 Size 4096
    [1] VA 0xfffffa8005373000 LA 0x117173000 !wdfcommonbuffer 0x57ffa65b9b8 Size 4096

    Event Ring TRBs:
        [207] TRANSFER_EVENT      0xfffffa8005373cf0 CycleBit 0 SlotId  2 EndpointID  4 EventData 1 Pointer 0xfffffa8005366700 CC_SUCCESS
        [208] TRANSFER_EVENT      0xfffffa8005373d00 CycleBit 0 SlotId  2 EndpointID  3 EventData 1 Pointer 0xfffffa8005a3d850 CC_SHORT_PACKET
        [209] TRANSFER_EVENT      0xfffffa8005373d10 CycleBit 0 SlotId  1 EndpointID  4 EventData 1 Pointer 0xfffffa8005a3d850 CC_SUCCESS
        [210] TRANSFER_EVENT      0xfffffa8005373d20 CycleBit 0 SlotId  1 EndpointID  3 EventData 1 Pointer 0xfffffa8005366700 CC_SUCCESS
        [211] TRANSFER_EVENT      0xfffffa8005373d30 CycleBit 0 SlotId  2 EndpointID  4 EventData 1 Pointer 0xfffffa8005366700 CC_SUCCESS
        [212] TRANSFER_EVENT      0xfffffa8005373d40 CycleBit 0 SlotId  2 EndpointID  3 EventData 1 Pointer 0xfffffa8005a3d850 CC_SHORT_PACKET
        [213] TRANSFER_EVENT      0xfffffa8005373d50 CycleBit 0 SlotId  1 EndpointID  4 EventData 1 Pointer 0xfffffa8005a3d850 CC_SUCCESS
        [214] TRANSFER_EVENT      0xfffffa8005373d60 CycleBit 0 SlotId  1 EndpointID  3 EventData 1 Pointer 0xfffffa8005366700 CC_SUCCESS
        [215] TRANSFER_EVENT      0xfffffa8005373d70 CycleBit 0 SlotId  2 EndpointID  4 EventData 1 Pointer 0xfffffa8005366700 CC_SUCCESS
        [216] TRANSFER_EVENT      0xfffffa8005373d80 CycleBit 0 SlotId  2 EndpointID  3 EventData 1 Pointer 0xfffffa8005a3d850 CC_SHORT_PACKET
```

## <span id="see_also"></span>See also


[USB 3.0 Extensions](usb-3-extensions.md)

[**!xhci\_dumpall**](-usb3kd-xhci-dumpall.md)

[Universal Serial Bus (USB) Drivers](http://go.microsoft.com/fwlink/p?LinkID=227351)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[debugger\debugger]:%20!usb3kd.xhci_eventring%20%20RELEASE:%20%285/15/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





