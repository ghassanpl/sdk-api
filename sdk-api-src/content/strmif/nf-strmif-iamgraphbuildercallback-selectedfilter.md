---
UID: NF:strmif.IAMGraphBuilderCallback.SelectedFilter
title: IAMGraphBuilderCallback::SelectedFilter (strmif.h)
description: The Filter Graph Manager calls this method when it finds a candidate filter for the graph, but before it creates the filter.
helpviewer_keywords: ["IAMGraphBuilderCallback interface [DirectShow]","SelectedFilter method","IAMGraphBuilderCallback.SelectedFilter","IAMGraphBuilderCallback::SelectedFilter","IAMGraphBuilderCallbackSelectedFilter","SelectedFilter","SelectedFilter method [DirectShow]","SelectedFilter method [DirectShow]","IAMGraphBuilderCallback interface","dshow.iamgraphbuildercallback_selectedfilter","strmif/IAMGraphBuilderCallback::SelectedFilter"]
old-location: dshow\iamgraphbuildercallback_selectedfilter.htm
tech.root: dshow
ms.assetid: a1768857-eb55-4b01-87af-921337a418c3
ms.date: 12/05/2018
ms.keywords: IAMGraphBuilderCallback interface [DirectShow],SelectedFilter method, IAMGraphBuilderCallback.SelectedFilter, IAMGraphBuilderCallback::SelectedFilter, IAMGraphBuilderCallbackSelectedFilter, SelectedFilter, SelectedFilter method [DirectShow], SelectedFilter method [DirectShow],IAMGraphBuilderCallback interface, dshow.iamgraphbuildercallback_selectedfilter, strmif/IAMGraphBuilderCallback::SelectedFilter
f1_keywords:
- strmif/IAMGraphBuilderCallback.SelectedFilter
dev_langs:
- c++
req.header: strmif.h
req.include-header: Dshow.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
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
- IAMGraphBuilderCallback.SelectedFilter
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IAMGraphBuilderCallback::SelectedFilter


## -description



The Filter Graph Manager calls this method when it finds a candidate filter for the graph, but before it creates the filter.




## -parameters




### -param pMon

Pointer to a moniker that contains information about the filter.


## -returns



If the method returns a success code, the Filter Graph Manager creates the filter and tries to connect it. If the method returns a failure code, the Filter Graph Manager rejects the filter.




## -remarks



This method enables the client to examine a filter to determine whether it is acceptable for the current filter graph.

The Filter Graph Manager holds a graph-wide critical section while it calls this method. Therefore, the callback method should avoid calling any methods on the Filter Graph Manager, or any methods on filters that might change the graph state (such as disconnecting pins). Doing so might cause a deadlock or other unexpected behaviors.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/strmif/nn-strmif-iamgraphbuildercallback">IAMGraphBuilderCallback Interface</a>
 

 

