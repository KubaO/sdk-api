---
UID: NF:directxmath.XMStoreFloat3x4
title: XMStoreFloat3x4
ms.date: 04/23/2020
description: Stores an [**XMMATRIX**](/windows/win32/api/directxmath/ns-directxmath-xmmatrix) in an [**XMFLOAT3X4**](/windows/win32/api/directxmath/ns-directxmath-xmfloat3x4).
tech.root: dxmath
f1_keywords:
- directxmath/XMStoreFloat3x4
dev_langs:
- c++
req.header: directxmath.h
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
- DirectXMath.h
api_name:
- XMStoreFloat3x4
targetos: Windows
req.typenames: 
req.redist: 
---

## -description

Stores an [**XMMATRIX**](/windows/win32/api/directxmath/ns-directxmath-xmmatrix) in an [**XMFLOAT3X4**](/windows/win32/api/directxmath/ns-directxmath-xmfloat3x4).

## -parameters

### -param pDestination [out]

Type: **XMFLOAT3X4 \*** 

Pointer to the [**XMFLOAT3X4**](/windows/win32/api/directxmath/ns-directxmath-xmfloat3x4) structure in which to store the data.

### -param M [in]

Type: **[XMMATRIX](/windows/win32/api/directxmath/ns-directxmath-xmmatrix)**

Matrix containing the data to store.

## -remarks

[**XMFLOAT3X4**](/windows/win32/api/directxmath/ns-directxmath-xmfloat3x4) is a row-major form of the matrix.

To write out column-major data requires that the [**XMMATRIX**](/windows/win32/api/directxmath/ns-directxmath-xmmatrix) be transposed via  [XMMatrixTranspose](/windows/win32/api/directxmath/nf-directxmath-xmmatrixtranspose) before calling the store function.

## -see-also
[DirectXMath Library vector store functions](/windows/win32/dxmath/ovw-xnamath-reference-functions-storage)