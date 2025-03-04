---
UID: NN:locationapi.ILocationEvents
title: ILocationEvents (locationapi.h)
description: ILocationEvents provides callback methods that you must implement if you want to receive event notifications.
helpviewer_keywords: ["ILocationEvents","ILocationEvents interface [WinLocation]","ILocationEvents interface [WinLocation]","described","locationapi/ILocationEvents","winlocation.ilocationevents"]
old-location: winlocation\ilocationevents.htm
tech.root: locationapi
ms.assetid: 5281ae0f-8599-4f84-a3f3-cde8c69e893d
ms.date: 12/05/2018
ms.keywords: ILocationEvents, ILocationEvents interface [WinLocation], ILocationEvents interface [WinLocation],described, locationapi/ILocationEvents, winlocation.ilocationevents
f1_keywords:
- locationapi/ILocationEvents
dev_langs:
- c++
req.header: locationapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7 [desktop apps only]
req.target-min-winversvr: None supported
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: LocationAPI.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- LocationAPI.dll
api_name:
- ILocationEvents
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ILocationEvents interface


## -description


<p class="CCE_Message">[The Win32 Location API is available for use in the operating systems specified in the Requirements section. It may be altered or unavailable in subsequent versions. Instead, use the <a href="https://docs.microsoft.com/uwp/api/windows.devices.geolocation">Windows.Devices.Geolocation</a>API.
]

<b>ILocationEvents</b> provides callback methods that 
    you must implement if you want to receive event notifications.
   


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">ILocationEvents</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>ILocationEvents</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>ILocationEvents</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/locationapi/nf-locationapi-ilocationevents-onlocationchanged">OnLocationChanged</a>
</td>
<td align="left" width="63%">
Called when a new location report is available.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/locationapi/nf-locationapi-ilocationevents-onstatuschanged">OnStatusChanged</a>
</td>
<td align="left" width="63%">
Called when a report status changes.

</td>
</tr>
</table> 

