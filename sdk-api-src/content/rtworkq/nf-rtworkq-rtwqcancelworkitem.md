---
UID: NF:rtworkq.RtwqCancelWorkItem
title: RtwqCancelWorkItem function (rtworkq.h)
description: Attempts to cancel an asynchronous operation that was scheduled with RtwqScheduleWorkItem.
helpviewer_keywords: ["RtwqCancelWorkItem","RtwqCancelWorkItem function","base.rtwqcancelworkitem","rtworkq/RtwqCancelWorkItem"]
old-location: base\rtwqcancelworkitem.htm
tech.root: ProcThread
ms.assetid: 55d5c6d6-310e-4f73-bbf4-9ac47a3ed295
ms.date: 12/05/2018
ms.keywords: RtwqCancelWorkItem, RtwqCancelWorkItem function, base.rtwqcancelworkitem, rtworkq/RtwqCancelWorkItem
f1_keywords:
- rtworkq/RtwqCancelWorkItem
dev_langs:
- c++
req.header: rtworkq.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8.1 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Rtworkq.lib
req.dll: RTWorkQ.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- RTWorkQ.dll
api_name:
- RtwqCancelWorkItem
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# RtwqCancelWorkItem function


## -description


Attempts to cancel an asynchronous operation that was scheduled with <a href="https://docs.microsoft.com/windows/desktop/api/rtworkq/nf-rtworkq-rtwqscheduleworkitem">RtwqScheduleWorkItem</a>.


## -parameters




### -param Key [in]

The key that was received in the <i>key</i> parameter of the <a href="https://docs.microsoft.com/windows/desktop/api/rtworkq/nf-rtworkq-rtwqscheduleworkitem">RtwqScheduleWorkItem</a>.
          


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Because work items are asynchronous, the  work-item callback might still be invoked after <b>RtwqCancelWorkItem</b> is called.



