---
UID: NF:directxcollision.BoundingOrientedBox.Intersects(FXMVECTOR,FXMVECTOR,float &)
title: BoundingOrientedBox::Intersects(FXMVECTOR,FXMVECTOR,float &)
description: Tests the BoundingOrientedBox for intersection with a ray.
helpviewer_keywords: ["BoundingOrientedBox interface [DirectX Math Support APIs]","Intersects method","BoundingOrientedBox.Intersects","BoundingOrientedBox.Intersects(FXMVECTOR","FXMVECTOR","float &)","BoundingOrientedBox.Intersects(XMVECTOR","XMVECTOR","float&)","BoundingOrientedBox::Intersects","BoundingOrientedBox::Intersects(FXMVECTOR","FXMVECTOR","float &)","Intersects","Intersects method [DirectX Math Support APIs]","Intersects method [DirectX Math Support APIs]","BoundingOrientedBox interface","dxmath.boundingorientedbox_intersects_2"]
old-location: dxmath\boundingorientedbox_intersects_2.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.directxmath.BoundingOrientedBox.Intersects(XMVECTOR,XMVECTOR,float@)
ms.date: 12/05/2018
ms.keywords: BoundingOrientedBox interface [DirectX Math Support APIs],Intersects method, BoundingOrientedBox.Intersects, BoundingOrientedBox.Intersects(FXMVECTOR,FXMVECTOR,float &), BoundingOrientedBox.Intersects(XMVECTOR,XMVECTOR,float&), BoundingOrientedBox::Intersects, BoundingOrientedBox::Intersects(FXMVECTOR,FXMVECTOR,float &), Intersects, Intersects method [DirectX Math Support APIs], Intersects method [DirectX Math Support APIs],BoundingOrientedBox interface, dxmath.boundingorientedbox_intersects_2
f1_keywords:
- directxcollision/BoundingOrientedBox.Intersects
dev_langs:
- c++
req.header: directxcollision.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
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
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- DirectXCollision.h
api_name:
- BoundingOrientedBox.Intersects
targetos: Windows
req.typenames: 
req.redist: 
---

# BoundingOrientedBox::Intersects(FXMVECTOR,FXMVECTOR,float &)


## -description


Tests the <a href="https://msdn.microsoft.com/ee1934f3-25ac-4a0e-84b9-6afcbdbef1f3">BoundingOrientedBox</a> for intersection with a ray.


## -parameters




### -param Origin [in]

The origin of the ray.


### -param Direction [in]

The direction of the ray.


### -param Dist [out, ref]

The length of the ray.


## -returns



A boolean value indicating whether the <a href="https://msdn.microsoft.com/ee1934f3-25ac-4a0e-84b9-6afcbdbef1f3">BoundingOrientedBox</a> intersects the ray.




## -remarks



<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.




## -see-also




<a href="https://msdn.microsoft.com/ee1934f3-25ac-4a0e-84b9-6afcbdbef1f3">BoundingOrientedBox</a>



<a href="https://msdn.microsoft.com/e9c23c95-631e-47df-b33e-b359fc75bac5">Intersects</a>



<b>Reference</b>
 

 

