---
UID: NF:msinkaut.IInkOverlay.SetGestureStatus
title: IInkOverlay::SetGestureStatus (msinkaut.h)
description: Sets the interest of the object or control in a known gesture.
helpviewer_keywords: ["7bab227f-d095-48e8-856f-6446e62826dd","IInkOverlay","IInkOverlay interface [Tablet PC]","SetGestureStatus method","IInkOverlay.SetGestureStatus","IInkOverlay::SetGestureStatus","SetGestureStatus","SetGestureStatus method [Tablet PC]","SetGestureStatus method [Tablet PC]","IInkOverlay interface","msinkaut/IInkOverlay::SetGestureStatus","tablet.inkoverlay_setgesturestatus"]
old-location: tablet\inkoverlay_setgesturestatus.htm
tech.root: tablet
ms.assetid: c55e0b19-257e-423f-bf84-3b7a55dc370e
ms.date: 12/05/2018
ms.keywords: 7bab227f-d095-48e8-856f-6446e62826dd, IInkOverlay, IInkOverlay interface [Tablet PC],SetGestureStatus method, IInkOverlay.SetGestureStatus, IInkOverlay::SetGestureStatus, SetGestureStatus, SetGestureStatus method [Tablet PC], SetGestureStatus method [Tablet PC],IInkOverlay interface, msinkaut/IInkOverlay::SetGestureStatus, tablet.inkoverlay_setgesturestatus
f1_keywords:
- msinkaut/IInkOverlay.SetGestureStatus
dev_langs:
- c++
req.header: msinkaut.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP Tablet PC Edition [desktop apps only]
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
req.lib: InkObj.dll
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- InkObj.dll
- InkObj.dll.dll
api_name:
- IInkOverlay.SetGestureStatus
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IInkOverlay::SetGestureStatus


## -description



Sets the interest of the object or control in a known gesture.




## -parameters




### -param Gesture [in]

The gesture that you want to set the status of.


### -param Listen [in]

<b>VARIANT_TRUE</b> if the gesture is being used or <b>VARIANT_FALSE</b> if it is being ignored.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Success.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
A parameter contained an invalid pointer.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_INVALID_MODE</b></dt>
</dl>
</td>
<td width="60%">
InkCollector collection mode must be in gesture mode.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INK_EXCEPTION</b></dt>
</dl>
</td>
<td width="60%">
An exception occurred.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>TPC_S_TRUNCATED</b></dt>
</dl>
</td>
<td width="60%">
Unsupported gesture.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The flag is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Cannot allocate memory operation.

</td>
</tr>
</table>
 




## -remarks



To get the interest of the object or control in a known gesture, call the <a href="https://docs.microsoft.com/windows/desktop/api/msinkaut/nf-msinkaut-iinkcollector-getgesturestatus">GetGestureStatus</a> method.

The <a href="https://docs.microsoft.com/windows/desktop/api/msinkaut/ne-msinkaut-inkapplicationgesture">IAG_AllGestures</a> gesture ID is not supported by the <a href="https://docs.microsoft.com/windows/desktop/tablet/inkedit-control-reference">InkEdit</a> control and returns an error. Passing invalid Gesture IDs does not return an error for InkEdit, but fails for <a href="https://docs.microsoft.com/windows/desktop/tablet/inkcollector-class">InkCollector</a>, <a href="https://docs.microsoft.com/windows/desktop/tablet/inkoverlay-class">InkOverlay</a>, and <a href="https://docs.microsoft.com/windows/desktop/tablet/inkpicture-control-reference">InkPicture</a>.

For the <a href="https://docs.microsoft.com/windows/desktop/tablet/inkedit-control-reference">InkEdit</a> control, this method should only be called if the <a href="https://docs.microsoft.com/windows/desktop/api/inked/nf-inked-iinkedit-get_status">Status</a> property returns <a href="https://docs.microsoft.com/windows/desktop/api/inked/ne-inked-inkeditstatus">IES_Idle</a>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/tablet/inkcollector-gesture">Gesture Event</a>



<a href="https://docs.microsoft.com/windows/desktop/api/msinkaut/nf-msinkaut-iinkcollector-getgesturestatus">GetGestureStatus Method</a>



<a href="https://msdn.microsoft.com/en-us/library/Mt846799(v=VS.85).aspx">IInkOverlay</a>



<a href="https://docs.microsoft.com/windows/desktop/api/msinkaut/ne-msinkaut-inkapplicationgesture">InkApplicationGesture Enumeration</a>



<a href="https://docs.microsoft.com/windows/desktop/tablet/inkoverlay-class">InkOverlay Class</a>
 

 

