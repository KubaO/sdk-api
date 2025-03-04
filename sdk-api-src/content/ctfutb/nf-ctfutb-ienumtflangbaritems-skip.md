---
UID: NF:ctfutb.IEnumTfLangBarItems.Skip
title: IEnumTfLangBarItems::Skip (ctfutb.h)
description: IEnumTfLangBarItems::Skip method
helpviewer_keywords: ["IEnumTfLangBarItems interface [Text Services Framework]","Skip method","IEnumTfLangBarItems.Skip","IEnumTfLangBarItems::Skip","Skip","Skip method [Text Services Framework]","Skip method [Text Services Framework]","IEnumTfLangBarItems interface","_tsf_ienumtflangbaritems_skip_ref","ctfutb/IEnumTfLangBarItems::Skip","tsf.ienumtflangbaritems_skip"]
old-location: tsf\ienumtflangbaritems_skip.htm
tech.root: TSF
ms.assetid: f9b4b899-1bcc-4ba5-a1e7-ca0a45749678
ms.date: 12/05/2018
ms.keywords: IEnumTfLangBarItems interface [Text Services Framework],Skip method, IEnumTfLangBarItems.Skip, IEnumTfLangBarItems::Skip, Skip, Skip method [Text Services Framework], Skip method [Text Services Framework],IEnumTfLangBarItems interface, _tsf_ienumtflangbaritems_skip_ref, ctfutb/IEnumTfLangBarItems::Skip, tsf.ienumtflangbaritems_skip
f1_keywords:
- ctfutb/IEnumTfLangBarItems.Skip
dev_langs:
- c++
req.header: ctfutb.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Ctfutb.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Msctf.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- msctf.dll
api_name:
- IEnumTfLangBarItems.Skip
targetos: Windows
req.typenames: 
req.redist: TSF 1.0 on Windows 2000 Professional
ms.custom: 19H1
---

# IEnumTfLangBarItems::Skip


## -description

Moves the current position forward in the enumeration sequence by the specified number of elements.

## -parameters




### -param ulCount [in]

Contains the number of elements to skip.


## -returns



This method can return one of these values.

<table>
<tr>
<th>Value</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_FALSE</b></dt>
</dl>
</td>
<td width="60%">
The method reached the end of the enumeration before the specified number of elements could be skipped.

</td>
</tr>
</table>
 



