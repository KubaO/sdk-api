---
UID: NF:gdiplusheaders.Region.Xor(IN const Rect &)
title: Region::Xor
description: The **Region::Xor** method updates a region to the nonintersecting portions with a rectangle's interior.
helpviewer_keywords: ["Region::Xor"]
ms.assetid: 06a4b045-996c-4f99-8bce-ec42ea09c170
ms.date: 05/20/2019
ms.keywords: Region::Xor
f1_keywords:
- gdiplusheaders/Region::Xor
dev_langs:
- c++
targetos: Windows
req.assembly: 
req.construct-type: function
req.ddi-compliance: 
req.dll: 
req.header: gdiplusheaders.h
req.idl: 
req.include-header: 
req.irql: 
req.kmdf-ver: 
req.lib: 
req.max-support: 
req.namespace: 
req.redist: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.target-type: 
req.type-library: 
req.umdf-ver: 
req.unicode-ansi: 
topic_type:
- apiref
api_type:
- COM
api_location:
- gdiplusheaders.h
api_name:
- Region::Xor
---

# Region::Xor(Rect&)

## -description

The **Region::Xor** method updates this region to the nonintersecting portions of itself and the specified rectangle's interior.

## -parameters

### -param rect

Reference to a rectangle to use to update this region.

## -returns

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a></b>

If the method succeeds, it returns Ok, which is an element of the <a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a> enumeration.

If the method fails, it returns one of the other elements of the <a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a> enumeration.

## -remarks

#### Examples

The following example creates a region from a path and then uses a rectangle to update the region.

```cpp
VOID Example_XorRect(HDC hdc)
{
   Graphics graphics(hdc);

  Point points[] = {
      Point(110, 20),
      Point(120, 30),
      Point(100, 60),
      Point(120, 70),
      Point(150, 60),
      Point(140, 10)};

   Rect rect(65, 15, 70, 45);
   GraphicsPath path;
   SolidBrush solidBrush(Color(255, 255, 0, 0));

   path.AddClosedCurve(points, 6);

   // Create a region from a path.
   Region pathRegion(&path);

   // Perform an exclusive OR operation on the region and a rectangle.
   pathRegion.Xor(rect);

   graphics.FillRegion(&solidBrush, &pathRegion);
}
```

## -see-also

<a href="https://docs.microsoft.com/windows/desktop/api/gdiplusheaders/nl-gdiplusheaders-region">Region</a>

<a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/nl-gdiplustypes-rect">Rect</a>

<a href="https://docs.microsoft.com/windows/desktop/api/gdiplustypes/ne-gdiplustypes-status">Status</a>
