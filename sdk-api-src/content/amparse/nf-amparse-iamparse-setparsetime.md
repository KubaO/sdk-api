---
UID: NF:amparse.IAMParse.SetParseTime
title: IAMParse::SetParseTime (amparse.h)
description: The SetParseTime method sets the current stream parse time. For MPEG-2, this corresponds to the system clock time computed for the current stream position.
helpviewer_keywords: ["IAMParse interface [DirectShow]","SetParseTime method","IAMParse.SetParseTime","IAMParse::SetParseTime","IAMParseSetParseTime","SetParseTime","SetParseTime method [DirectShow]","SetParseTime method [DirectShow]","IAMParse interface","amparse/IAMParse::SetParseTime","dshow.iamparse_setparsetime"]
old-location: dshow\iamparse_setparsetime.htm
tech.root: DirectShow
ms.assetid: 52c53994-7cb7-4f50-a00d-87faa309c717
ms.date: 12/05/2018
ms.keywords: IAMParse interface [DirectShow],SetParseTime method, IAMParse.SetParseTime, IAMParse::SetParseTime, IAMParseSetParseTime, SetParseTime, SetParseTime method [DirectShow], SetParseTime method [DirectShow],IAMParse interface, amparse/IAMParse::SetParseTime, dshow.iamparse_setparsetime
f1_keywords:
- amparse/IAMParse.SetParseTime
dev_langs:
- c++
req.header: amparse.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Strmiids.lib
- Strmiids.dll
api_name:
- IAMParse.SetParseTime
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAMParse::SetParseTime


## -description



The <code>SetParseTime</code> method sets the current stream parse time. For MPEG-2, this corresponds to the system clock time computed for the current stream position.




## -parameters




### -param rtCurrent [in]

Current stream parse time.


## -returns



Returns an <b>HRESULT</b> value. Possible values include the following.

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
<dt><b>VFW_E_NOT_CONNECTED</b></dt>
</dl>
</td>
<td width="60%">
The parse time is not available, because the input pin is not connected

</td>
</tr>
</table>
 




## -remarks



The parse time for the MPEG-2 Splitter filter is the current stream position in system clock units. The initial value of the parse time is zero.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/error-and-success-codes">Error and Success Codes</a>



<a href="https://docs.microsoft.com/windows/desktop/api/amparse/nn-amparse-iamparse">IAMParse Interface</a>
 

 

