---
UID: NF:atscpsipparser.IATSC_MGT.GetRecordCountOfDescriptors
title: IATSC_MGT::GetRecordCountOfDescriptors (atscpsipparser.h)
description: This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
helpviewer_keywords: ["GetRecordCountOfDescriptors","GetRecordCountOfDescriptors method [Microsoft TV Technologies]","GetRecordCountOfDescriptors method [Microsoft TV Technologies]","IATSC_MGT interface","IATSC_MGT interface [Microsoft TV Technologies]","GetRecordCountOfDescriptors method","IATSC_MGT.GetRecordCountOfDescriptors","IATSC_MGT::GetRecordCountOfDescriptors","IATSC_MGTGetRecordCountOfDescriptors","atscpsipparser/IATSC_MGT::GetRecordCountOfDescriptors","mstv.iatsc_mgt_getrecordcountofdescriptors"]
old-location: mstv\iatsc_mgt_getrecordcountofdescriptors.htm
tech.root: mstv
ms.assetid: 66be731b-d964-4806-ae78-2faa0c0d2810
ms.date: 12/05/2018
ms.keywords: GetRecordCountOfDescriptors, GetRecordCountOfDescriptors method [Microsoft TV Technologies], GetRecordCountOfDescriptors method [Microsoft TV Technologies],IATSC_MGT interface, IATSC_MGT interface [Microsoft TV Technologies],GetRecordCountOfDescriptors method, IATSC_MGT.GetRecordCountOfDescriptors, IATSC_MGT::GetRecordCountOfDescriptors, IATSC_MGTGetRecordCountOfDescriptors, atscpsipparser/IATSC_MGT::GetRecordCountOfDescriptors, mstv.iatsc_mgt_getrecordcountofdescriptors
f1_keywords:
- atscpsipparser/IATSC_MGT.GetRecordCountOfDescriptors
dev_langs:
- c++
req.header: atscpsipparser.h
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
- atscpsipparser.h
api_name:
- IATSC_MGT.GetRecordCountOfDescriptors
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IATSC_MGT::GetRecordCountOfDescriptors


## -description



This topic applies to Update Rollup 2 for Microsoft Windows XP Media Center Edition 2005 and later.
        



The <b>GetRecordCountOfDescriptors</b> method returns the number of descriptors for a record in the MGT.


## -parameters




### -param dwRecordIndex [in]

Specifies the record number, indexed from zero. Call the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/atscpsipparser/nf-atscpsipparser-iatsc_mgt-getcountofrecords">IATSC_MGT::GetCountOfRecords</a> method to get the number of records in the MGT.


### -param pdwVal [out]

Receives the number of descriptors.


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
<dt><b>MPEG2_E_OUT_OF_BOUNDS</b></dt>
</dl>
</td>
<td width="60%">
Index out of bounds.

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




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/atscpsipparser/nn-atscpsipparser-iatsc_mgt">IATSC_MGT Interface</a>
 

 

