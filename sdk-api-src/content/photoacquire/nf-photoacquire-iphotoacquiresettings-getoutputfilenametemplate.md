---
UID: NF:photoacquire.IPhotoAcquireSettings.GetOutputFilenameTemplate
title: IPhotoAcquireSettings::GetOutputFilenameTemplate (photoacquire.h)
description: The GetOutputFilenameTemplate method retrieves a format string (template) that specifies the format of file names.
helpviewer_keywords: ["GetOutputFilenameTemplate","GetOutputFilenameTemplate method [Picture Acquisition]","GetOutputFilenameTemplate method [Picture Acquisition]","IPhotoAcquireSettings interface","IPhotoAcquireSettings interface [Picture Acquisition]","GetOutputFilenameTemplate method","IPhotoAcquireSettings.GetOutputFilenameTemplate","IPhotoAcquireSettings::GetOutputFilenameTemplate","IPhotoAcquireSettingsGetOutputFilenameTemplate","photoacquire/IPhotoAcquireSettings::GetOutputFilenameTemplate","picacq.iphotoacquiresettings_getoutputfilenametemplate"]
old-location: picacq\iphotoacquiresettings_getoutputfilenametemplate.htm
tech.root: acquisition
ms.assetid: ca36e3f9-74ad-4704-adeb-d3102668da30
ms.date: 12/05/2018
ms.keywords: GetOutputFilenameTemplate, GetOutputFilenameTemplate method [Picture Acquisition], GetOutputFilenameTemplate method [Picture Acquisition],IPhotoAcquireSettings interface, IPhotoAcquireSettings interface [Picture Acquisition],GetOutputFilenameTemplate method, IPhotoAcquireSettings.GetOutputFilenameTemplate, IPhotoAcquireSettings::GetOutputFilenameTemplate, IPhotoAcquireSettingsGetOutputFilenameTemplate, photoacquire/IPhotoAcquireSettings::GetOutputFilenameTemplate, picacq.iphotoacquiresettings_getoutputfilenametemplate
f1_keywords:
- photoacquire/IPhotoAcquireSettings.GetOutputFilenameTemplate
dev_langs:
- c++
req.header: photoacquire.h
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
req.lib: PhotoAcquireUID.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- PhotoAcquireUID.lib
- PhotoAcquireUID.dll
api_name:
- IPhotoAcquireSettings.GetOutputFilenameTemplate
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IPhotoAcquireSettings::GetOutputFilenameTemplate


## -description



The <code>GetOutputFilenameTemplate</code> method retrieves a format string (template) that specifies the format of file names.




## -parameters




### -param pbstrTemplate [out]

Pointer to a string containing the format string.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



Format strings contain a mix of path literals and tokens. A format string looks like the following:

<pre class="syntax" xml:space="preserve"><code>
$(MyPicturesFolder)\$(DateAcquired), $(EventName)\$(EventName) $(SequenceNumber).$(OriginalExtension)
</code></pre>



## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/photoacquire/nn-photoacquire-iphotoacquiresettings">IPhotoAcquireSettings Interface</a>



<a href="https://docs.microsoft.com/windows/desktop/api/photoacquire/nf-photoacquire-iphotoacquiresettings-setoutputfilenametemplate">SetOutputFilenameTemplate</a>
 

 

