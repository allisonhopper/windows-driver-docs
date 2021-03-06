---
title: Custom UI Design Information
description: Custom UI Design Information
ms.assetid: ec1da6d4-a357-4e23-a476-885fbf6441b7
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# Custom UI Design Information


If you design your own sAPOs to replace the system-supplied sAPOs, you must provide a custom user interface for configuring the system effects features of your sAPO.

In this case, the user interface will not be a replacement for the system-supplied **Enhancements** property page. And adding a new property page to the **Sound** applet in the Control Panel, involves adding a new tab to the system-supplied **Sound** applet. This means that when the custom sAPOs are registered and initialized, their property page will be available along with the system-supplied **Enhancements** page. It is difficult and complicated to implement communication across the property pages of two different sAPOs. So it is possible that some default settings on the **Enhancements** page will conflict with feature settings on the new property page.

Therefore the most practical approach here is to implement a separate UI for configuring the custom sAPOs that you developed to replace the system-supplied sAPOs. To develop and implement your custom UI, perform the following steps.

1.  [Develop a custom UI](http://go.microsoft.com/fwlink/p/?linkid=106006) for configuring your system effects features

2.  [Create a DLL](http://go.microsoft.com/fwlink/p/?linkid=106014) package from your custom UI

3.  Create or modify an [INF file](https://msdn.microsoft.com/library/windows/hardware/ff549520) for installing and registering your DLL

 

 


--------------------
[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[audio\audio]:%20Custom%20UI%20Design%20Information%20%20RELEASE:%20%287/18/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")


