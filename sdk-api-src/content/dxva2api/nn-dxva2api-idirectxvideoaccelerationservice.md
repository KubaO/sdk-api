---
UID: NN:dxva2api.IDirectXVideoAccelerationService
title: IDirectXVideoAccelerationService (dxva2api.h)
description: Provides DirectX Video Acceleration (DXVA) services from a Direct3D device.
helpviewer_keywords: ["50a2d8f7-d7c9-4d50-88cc-f6c8562fbb17","IDirectXVideoAccelerationService","IDirectXVideoAccelerationService interface [Media Foundation]","IDirectXVideoAccelerationService interface [Media Foundation]","described","dxva2api/IDirectXVideoAccelerationService","mf.idirectxvideoaccelerationservice"]
old-location: mf\idirectxvideoaccelerationservice.htm
tech.root: medfound
ms.assetid: 50a2d8f7-d7c9-4d50-88cc-f6c8562fbb17
ms.date: 12/05/2018
ms.keywords: 50a2d8f7-d7c9-4d50-88cc-f6c8562fbb17, IDirectXVideoAccelerationService, IDirectXVideoAccelerationService interface [Media Foundation], IDirectXVideoAccelerationService interface [Media Foundation],described, dxva2api/IDirectXVideoAccelerationService, mf.idirectxvideoaccelerationservice
f1_keywords:
- dxva2api/IDirectXVideoAccelerationService
dev_langs:
- c++
req.header: dxva2api.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- dxva2api.h
api_name:
- IDirectXVideoAccelerationService
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDirectXVideoAccelerationService interface


## -description


Provides DirectX Video Acceleration (DXVA) services from a Direct3D device. To get a pointer to this interface, call <a href="https://docs.microsoft.com/windows/desktop/api/dxva2api/nf-dxva2api-idirect3ddevicemanager9-getvideoservice">IDirect3DDeviceManager9::GetVideoService</a> or <a href="https://docs.microsoft.com/windows/desktop/api/dxva2api/nf-dxva2api-dxva2createvideoservice">DXVA2CreateVideoService</a>.


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IDirectXVideoAccelerationService</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IDirectXVideoAccelerationService</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IDirectXVideoAccelerationService</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/dxva2api/nf-dxva2api-idirectxvideoaccelerationservice-createsurface">CreateSurface</a>
</td>
<td align="left" width="63%">
Creates a DirectX Video Acceleration (DXVA) video processor or DXVA decoder render target.
        

</td>
</tr>
</table> 


## -remarks



This is the base interface for DXVA services. The Direct3D device can support any of the following DXVA services, which derive from <b>IDirectXVideoAccelerationService</b>:

<ul>
<li>Video decoding: <a href="https://docs.microsoft.com/windows/desktop/api/dxva2api/nn-dxva2api-idirectxvideodecoderservice">IDirectXVideoDecoderService</a>
</li>
<li>Video processing: <a href="https://docs.microsoft.com/windows/desktop/api/dxva2api/nn-dxva2api-idirectxvideoprocessorservice">IDirectXVideoProcessorService</a>
</li>
</ul>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/medfound/directx-video-acceleration-2-0">DirectX Video Acceleration 2.0</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/media-foundation-interfaces">Media Foundation Interfaces</a>
 

 

