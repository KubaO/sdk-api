---
UID: NF:d3d11_1.ID3D11RasterizerState1.GetDesc1
title: ID3D11RasterizerState1::GetDesc1 (d3d11_1.h)
description: Gets the description for rasterizer state that you used to create the rasterizer-state object.
helpviewer_keywords: ["GetDesc1","GetDesc1 method [Direct3D 11]","GetDesc1 method [Direct3D 11]","ID3D11RasterizerState1 interface","ID3D11RasterizerState1 interface [Direct3D 11]","GetDesc1 method","ID3D11RasterizerState1.GetDesc1","ID3D11RasterizerState1::GetDesc1","d3d11_1/ID3D11RasterizerState1::GetDesc1","direct3d11.id3d11rasterizerstate1_getdesc1"]
old-location: direct3d11\id3d11rasterizerstate1_getdesc1.htm
tech.root: direct3d11
ms.assetid: A16EFA79-6138-4F3B-B4ED-E525C07DD4EF
ms.date: 12/05/2018
ms.keywords: GetDesc1, GetDesc1 method [Direct3D 11], GetDesc1 method [Direct3D 11],ID3D11RasterizerState1 interface, ID3D11RasterizerState1 interface [Direct3D 11],GetDesc1 method, ID3D11RasterizerState1.GetDesc1, ID3D11RasterizerState1::GetDesc1, d3d11_1/ID3D11RasterizerState1::GetDesc1, direct3d11.id3d11rasterizerstate1_getdesc1
f1_keywords:
- d3d11_1/ID3D11RasterizerState1.GetDesc1
dev_langs:
- c++
req.header: d3d11_1.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 and Platform Update for Windows 7 [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2012 and Platform Update for Windows Server 2008 R2 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: D3D11.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D3D11.lib
- D3D11.dll
api_name:
- ID3D11RasterizerState1.GetDesc1
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# ID3D11RasterizerState1::GetDesc1


## -description


Gets the description for rasterizer state that you used to create the rasterizer-state object.


## -parameters




### -param pDesc [out]

A pointer to a <a href="https://docs.microsoft.com/windows/desktop/api/d3d11_1/ns-d3d11_1-cd3d11_rasterizer_desc1">D3D11_RASTERIZER_DESC1</a> structure that receives a description of the rasterizer state. This rasterizer state can specify forced sample count.


## -remarks



You use the description for rasterizer state in a call to the <a href="https://docs.microsoft.com/windows/desktop/api/d3d11_1/nf-d3d11_1-id3d11device1-createrasterizerstate1">ID3D11Device1::CreateRasterizerState1</a> method to create the rasterizer-state object.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/d3d11_1/nn-d3d11_1-id3d11rasterizerstate1">ID3D11RasterizerState1</a>
 

 

