---
UID: NF:dvbsiparser.IIsdbDownloadContentDescriptor.GetComponentSize
title: IIsdbDownloadContentDescriptor::GetComponentSize (dvbsiparser.h)
description: Gets the total size of components transmitted within the same carousel from an Integrated Services Digital Broadcasting (ISDB) download content descriptor, in bytes.
helpviewer_keywords: ["GetComponentSize","GetComponentSize method [Microsoft TV Technologies]","GetComponentSize method [Microsoft TV Technologies]","IIsdbDownloadContentDescriptor interface","IIsdbDownloadContentDescriptor interface [Microsoft TV Technologies]","GetComponentSize method","IIsdbDownloadContentDescriptor.GetComponentSize","IIsdbDownloadContentDescriptor::GetComponentSize","dvbsiparser/IIsdbDownloadContentDescriptor::GetComponentSize","mstv.iisdbdownloadcontentdescriptor_getcomponentsize"]
old-location: mstv\iisdbdownloadcontentdescriptor_getcomponentsize.htm
tech.root: mstv
ms.assetid: 07edb403-6674-4673-928c-91e7df9fe9da
ms.date: 12/05/2018
ms.keywords: GetComponentSize, GetComponentSize method [Microsoft TV Technologies], GetComponentSize method [Microsoft TV Technologies],IIsdbDownloadContentDescriptor interface, IIsdbDownloadContentDescriptor interface [Microsoft TV Technologies],GetComponentSize method, IIsdbDownloadContentDescriptor.GetComponentSize, IIsdbDownloadContentDescriptor::GetComponentSize, dvbsiparser/IIsdbDownloadContentDescriptor::GetComponentSize, mstv.iisdbdownloadcontentdescriptor_getcomponentsize
f1_keywords:
- dvbsiparser/IIsdbDownloadContentDescriptor.GetComponentSize
dev_langs:
- c++
req.header: dvbsiparser.h
req.include-header: Dvbsiparser.idl
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
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- dvbsiparser.h
api_name:
- IIsdbDownloadContentDescriptor.GetComponentSize
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IIsdbDownloadContentDescriptor::GetComponentSize


## -description


Gets the total size of components transmitted within the same carousel from an Integrated Services Digital Broadcasting (ISDB) download content descriptor, in bytes.


## -parameters




### -param pdwVal [out]

Receives the component size.


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/dvbsiparser/nn-dvbsiparser-iisdbdownloadcontentdescriptor">IIsdbDownloadContentDescriptor</a>
 

 

