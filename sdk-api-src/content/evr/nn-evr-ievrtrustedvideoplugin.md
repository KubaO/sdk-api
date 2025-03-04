---
UID: NN:evr.IEVRTrustedVideoPlugin
title: IEVRTrustedVideoPlugin (evr.h)
description: Enables a plug-in component for the enhanced video renderer (EVR) to work with protected media.
helpviewer_keywords: ["1dcaa01c-2596-4a22-9e2a-7f0e26d58ffe","IEVRTrustedVideoPlugin","IEVRTrustedVideoPlugin interface [Media Foundation]","IEVRTrustedVideoPlugin interface [Media Foundation]","described","evr/IEVRTrustedVideoPlugin","mf.ievrtrustedvideoplugin"]
old-location: mf\ievrtrustedvideoplugin.htm
tech.root: medfound
ms.assetid: 1dcaa01c-2596-4a22-9e2a-7f0e26d58ffe
ms.date: 12/05/2018
ms.keywords: 1dcaa01c-2596-4a22-9e2a-7f0e26d58ffe, IEVRTrustedVideoPlugin, IEVRTrustedVideoPlugin interface [Media Foundation], IEVRTrustedVideoPlugin interface [Media Foundation],described, evr/IEVRTrustedVideoPlugin, mf.ievrtrustedvideoplugin
f1_keywords:
- evr/IEVRTrustedVideoPlugin
dev_langs:
- c++
req.header: evr.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Mfuuid.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- mfuuid.lib
- mfuuid.dll
api_name:
- IEVRTrustedVideoPlugin
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IEVRTrustedVideoPlugin interface


## -description


Enables a plug-in component for the enhanced video renderer (EVR) to work with protected media.

To work in the protected media path (PMP), a custom EVR mixer or presenter must implement this interface. The EVR obtains a pointer to this interface by calling <b>QueryInterface</b> on the plug-in component.

This interface is required only if the plug-in is a trusted component, designed to work in the PMP. It is not required for playing clear content in an unprotected process.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IEVRTrustedVideoPlugin</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IEVRTrustedVideoPlugin</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IEVRTrustedVideoPlugin</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/evr/nf-evr-ievrtrustedvideoplugin-canconstrict">CanConstrict</a>
</td>
<td align="left" width="63%">
Queries whether the plug-in can limit the effective video resolution.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/evr/nf-evr-ievrtrustedvideoplugin-disableimageexport">DisableImageExport</a>
</td>
<td align="left" width="63%">
Enables or disables the ability of the plug-in to export the video image.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/evr/nf-evr-ievrtrustedvideoplugin-isintrustedvideomode">IsInTrustedVideoMode</a>
</td>
<td align="left" width="63%">
Queries whether the plug-in has any transient vulnerabilities at this time.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/evr/nf-evr-ievrtrustedvideoplugin-setconstriction">SetConstriction</a>
</td>
<td align="left" width="63%">
Limits the effective video resolution.

</td>
</tr>
</table> 


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/medfound/enhanced-video-renderer">Enhanced Video Renderer</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/media-foundation-interfaces">Media Foundation Interfaces</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/protected-media-path">Protected Media Path</a>
 

 

