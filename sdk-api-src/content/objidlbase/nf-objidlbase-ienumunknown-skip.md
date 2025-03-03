---
UID: NF:objidlbase.IEnumUnknown.Skip
title: IEnumUnknown::Skip (objidlbase.h)
description: Skips over the specified number of items in the enumeration sequence.
helpviewer_keywords: ["IEnumUnknown interface [COM]","Skip method","IEnumUnknown.Skip","IEnumUnknown::Skip","Skip","Skip method [COM]","Skip method [COM]","IEnumUnknown interface","_com_ienumunknown_skip","com.ienumunknown_skip","objidlbase/IEnumUnknown::Skip"]
old-location: com\ienumunknown_skip.htm
tech.root: com
ms.assetid: 6d73a119-0da8-4754-92c3-53f75d7be9e0
ms.date: 12/05/2018
ms.keywords: IEnumUnknown interface [COM],Skip method, IEnumUnknown.Skip, IEnumUnknown::Skip, Skip, Skip method [COM], Skip method [COM],IEnumUnknown interface, _com_ienumunknown_skip, com.ienumunknown_skip, objidlbase/IEnumUnknown::Skip
f1_keywords:
- objidlbase/IEnumUnknown.Skip
dev_langs:
- c++
req.header: objidlbase.h
req.include-header: ObjIdl.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps \| UWP apps]
req.target-min-winversvr: Windows 2000 Server [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: ObjIdl.idl
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
- objidlbase.h
api_name:
- IEnumUnknown.Skip
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IEnumUnknown::Skip


## -description


Skips over the specified number of items in the enumeration sequence.


## -parameters




### -param celt [in]

The number of items to be skipped.


## -returns



If the method skips the number of items requested, the return value is S_OK. Otherwise, it is S_FALSE.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/objidl/nn-objidl-ienumunknown">IEnumUnknown</a>
 

 

