---
UID: NF:dvbsiparser.IDVB_SDT.Initialize
title: IDVB_SDT::Initialize (dvbsiparser.h)
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
helpviewer_keywords: ["IDVB_SDT interface [Microsoft TV Technologies]","Initialize method","IDVB_SDT.Initialize","IDVB_SDT::Initialize","IDVB_SDTInitialize","Initialize","Initialize method [Microsoft TV Technologies]","Initialize method [Microsoft TV Technologies]","IDVB_SDT interface","dvbsiparser/IDVB_SDT::Initialize","mstv.idvb_sdt_initialize"]
old-location: mstv\idvb_sdt_initialize.htm
tech.root: mstv
ms.assetid: f9e3bfb8-e879-4016-bd4d-f2a0d4d44938
ms.date: 12/05/2018
ms.keywords: IDVB_SDT interface [Microsoft TV Technologies],Initialize method, IDVB_SDT.Initialize, IDVB_SDT::Initialize, IDVB_SDTInitialize, Initialize, Initialize method [Microsoft TV Technologies], Initialize method [Microsoft TV Technologies],IDVB_SDT interface, dvbsiparser/IDVB_SDT::Initialize, mstv.idvb_sdt_initialize
f1_keywords:
- dvbsiparser/IDVB_SDT.Initialize
dev_langs:
- c++
req.header: dvbsiparser.h
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
- dvbsiparser.h
api_name:
- IDVB_SDT.Initialize
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDVB_SDT::Initialize


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>Initialize</b> method initializes the object using captured table section data. This method is called internally by the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/dvbsiparser/nf-dvbsiparser-idvbsiparser-getsdt">IDvbSiParser::GetSDT</a> method, so applications typically should not call it.


## -parameters




### -param pSectionList [in]

Pointer to the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/mpeg2data/nn-mpeg2data-isectionlist">ISectionList</a> interface of the <b>SectionList</b> object that contains the section data.


### -param pMPEGData [in]

Pointer to the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/mpeg2data/nn-mpeg2data-impeg2data">IMpeg2Data</a> interface of the MPEG-2 Sections and Tables filter.


## -returns



The method returns an <b>HRESULT</b>. Possible values include those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
Invalid argument.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>MPEG2_E_ALREADY_INITIALIZED</b></dt>
</dl>
</td>
<td width="60%">
The object is already initialized.

</td>
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
 




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/dvbsiparser/nn-dvbsiparser-idvb_sdt">IDVB_SDT Interface</a>
 

 

