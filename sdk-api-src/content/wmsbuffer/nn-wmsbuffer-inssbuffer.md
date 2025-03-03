---
UID: NN:wmsbuffer.INSSBuffer
title: INSSBuffer (wmsbuffer.h)
description: The INSSBuffer interface is the basic interface of a buffer object.
helpviewer_keywords: ["INSSBuffer","INSSBuffer interface [windows Media Format]","INSSBuffer interface [windows Media Format]","described","INSSBufferInterface","wmformat.inssbuffer","wmsbuffer/INSSBuffer"]
old-location: wmformat\inssbuffer.htm
tech.root: wmformat
ms.assetid: c47c016a-e7eb-4a2c-b365-5537749db5bc
ms.date: 12/05/2018
ms.keywords: INSSBuffer, INSSBuffer interface [windows Media Format], INSSBuffer interface [windows Media Format],described, INSSBufferInterface, wmformat.inssbuffer, wmsbuffer/INSSBuffer
f1_keywords:
- wmsbuffer/INSSBuffer
dev_langs:
- c++
req.header: wmsbuffer.h
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
- wmsbuffer.h
api_name:
- INSSBuffer
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# INSSBuffer interface


## -description



The <b>INSSBuffer</b> interface is the basic interface of a buffer object. A buffer object is a wrapper around a memory buffer. The methods exposed by this interface are used to manipulate the buffer.

In both writing and reading ASF files, buffer objects are used to contain samples. Depending upon where you use a sample, you will obtain a reference to the <b>INSSBuffer</b> interface in one of three ways:

<ul>
<li>When passing samples to the writer, you can obtain buffer objects by calling <a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmwriter-allocatesample">IWMWriter::AllocateSample</a>.</li>
<li>When you are receiving samples from the asynchronous reader, buffer objects are created automatically, and references to an <b>INSSBuffer</b> interface are passed with every call the reader makes to the <a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmreadercallback-onsample">IWMReaderCallback::OnSample</a> callback method.</li>
<li>When you are receiving samples from the synchronous reader, a reference to an <b>INSSBuffer</b> interface is set with every call you make to <a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmsyncreader-getnextsample">IWMSyncReader::GetNextSample</a>.</li>
</ul>


The following interfaces can be obtained by using the QueryInterface method of this interface.
<table>
<tr>
<th>Interface</th>
<th>IID</th>
</tr>
<tr>
<td>
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer2">INSSBuffer2</a>
</td>
<td>IID_INSSBuffer2</td>
</tr>
<tr>
<td>
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer3">INSSBuffer3</a>
</td>
<td>IID_INSSBuffer3</td>
</tr>
<tr>
<td>
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nn-wmsbuffer-inssbuffer4">INSSBuffer4</a>
</td>
<td>IID_INSSBuffer4</td>
</tr>
</table>
 




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">INSSBuffer</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>INSSBuffer</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>INSSBuffer</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer-getbuffer">GetBuffer</a>
</td>
<td align="left" width="63%">
Retrieves the location of the buffer.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer-getbufferandlength">GetBufferAndLength</a>
</td>
<td align="left" width="63%">
Retrieves the location and size of the used portion of the buffer.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer-getlength">GetLength</a>
</td>
<td align="left" width="63%">
Retrieves the size of the used portion of the buffer.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer-getmaxlength">GetMaxLength</a>
</td>
<td align="left" width="63%">
Retrieves the maximum size to which a buffer can be set.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/wmsbuffer/nf-wmsbuffer-inssbuffer-setlength">SetLength</a>
</td>
<td align="left" width="63%">
Specifies the size of the used portion of the buffer.

</td>
</tr>
</table> 


## -see-also




<a href="https://docs.microsoft.com/windows/desktop/wmformat/buffer-object">Buffer Object</a>



<a href="https://docs.microsoft.com/windows/desktop/wmformat/interfaces">Interfaces</a>



<a href="https://docs.microsoft.com/windows/desktop/wmformat/reading-asf-files">Reading ASF Files</a>



<a href="https://docs.microsoft.com/windows/desktop/wmformat/writing-asf-files">Writing ASF Files</a>
 

 

