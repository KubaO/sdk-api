---
UID: NN:mfidl.IMFStreamDescriptor
title: IMFStreamDescriptor (mfidl.h)
description: Gets information about one stream in a media source.
helpviewer_keywords: ["IMFStreamDescriptor","IMFStreamDescriptor interface [Media Foundation]","IMFStreamDescriptor interface [Media Foundation]","described","a076dc6e-d9cb-4f7e-8cc2-b66292da295f","mf.imfstreamdescriptor","mfidl/IMFStreamDescriptor"]
old-location: mf\imfstreamdescriptor.htm
tech.root: medfound
ms.assetid: a076dc6e-d9cb-4f7e-8cc2-b66292da295f
ms.date: 12/05/2018
ms.keywords: IMFStreamDescriptor, IMFStreamDescriptor interface [Media Foundation], IMFStreamDescriptor interface [Media Foundation],described, a076dc6e-d9cb-4f7e-8cc2-b66292da295f, mf.imfstreamdescriptor, mfidl/IMFStreamDescriptor
f1_keywords:
- mfidl/IMFStreamDescriptor
dev_langs:
- c++
req.header: mfidl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 [desktop apps \| UWP apps]
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
- IMFStreamDescriptor
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IMFStreamDescriptor interface


## -description


Gets information about one stream in a media source.
        


## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IMFStreamDescriptor</b> interface inherits from <a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes">IMFAttributes</a>. <b>IMFStreamDescriptor</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IMFStreamDescriptor</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nf-mfidl-imfstreamdescriptor-getmediatypehandler">GetMediaTypeHandler</a>
</td>
<td align="left" width="63%">
Retrieves a media type handler that can be used to enumerate and set media types for the stream.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nf-mfidl-imfstreamdescriptor-getstreamidentifier">GetStreamIdentifier</a>
</td>
<td align="left" width="63%">
Retrieves an identifier for the stream.

</td>
</tr>
</table> 


## -remarks



A presentation descriptor contains one or more stream descriptors. To get the stream descriptors from a presentation descriptor, call <a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nf-mfidl-imfpresentationdescriptor-getstreamdescriptorbyindex">IMFPresentationDescriptor::GetStreamDescriptorByIndex</a>. To create a new stream descriptor, call <a href="https://docs.microsoft.com/windows/desktop/api/mfidl/nf-mfidl-mfcreatestreamdescriptor">MFCreateStreamDescriptor</a>.

This interface is available on the following platforms if the Windows Media Format 11 SDK redistributable components are installed:

<ul>
<li>Windows XP with Service Pack 2 (SP2) and later.</li>
<li>Windows XP Media Center Edition 2005 with KB900325 (Windows XP Media Center Edition 2005) and KB925766 (October 2006 Update Rollup for Windows XP Media Center Edition) installed.</li>
</ul>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/mfobjects/nn-mfobjects-imfattributes">IMFAttributes</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/media-foundation-interfaces">Media Foundation Interfaces</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/presentation-descriptors">Presentation Descriptors</a>



<a href="https://docs.microsoft.com/windows/desktop/medfound/stream-descriptor-attributes">Stream Descriptor Attributes</a>
 

 

