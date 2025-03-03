---
UID: NF:wmsdkidl.IWMReaderNetworkConfig.SetEnableMulticast
title: IWMReaderNetworkConfig::SetEnableMulticast (wmsdkidl.h)
description: The SetEnableMulticast method enables or disables multicasting.
helpviewer_keywords: ["IWMReaderNetworkConfig interface [windows Media Format]","SetEnableMulticast method","IWMReaderNetworkConfig.SetEnableMulticast","IWMReaderNetworkConfig::SetEnableMulticast","IWMReaderNetworkConfigSetEnableMulticast","SetEnableMulticast","SetEnableMulticast method [windows Media Format]","SetEnableMulticast method [windows Media Format]","IWMReaderNetworkConfig interface","wmformat.iwmreadernetworkconfig_setenablemulticast","wmsdkidl/IWMReaderNetworkConfig::SetEnableMulticast"]
old-location: wmformat\iwmreadernetworkconfig_setenablemulticast.htm
tech.root: wmformat
ms.assetid: 02e3a7cc-1dcf-4aba-a18f-2056742f0777
ms.date: 12/05/2018
ms.keywords: IWMReaderNetworkConfig interface [windows Media Format],SetEnableMulticast method, IWMReaderNetworkConfig.SetEnableMulticast, IWMReaderNetworkConfig::SetEnableMulticast, IWMReaderNetworkConfigSetEnableMulticast, SetEnableMulticast, SetEnableMulticast method [windows Media Format], SetEnableMulticast method [windows Media Format],IWMReaderNetworkConfig interface, wmformat.iwmreadernetworkconfig_setenablemulticast, wmsdkidl/IWMReaderNetworkConfig::SetEnableMulticast
f1_keywords:
- wmsdkidl/IWMReaderNetworkConfig.SetEnableMulticast
dev_langs:
- c++
req.header: wmsdkidl.h
req.include-header: Wmsdk.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only],Windows Media Format 7 SDK, or later versions of the SDK
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
req.lib: Wmvcore.lib; WMStubDRM.lib (if you use DRM)
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Wmvcore.lib
- Wmvcore.dll
- WMStubDRM.lib
- WMStubDRM.dll
api_name:
- IWMReaderNetworkConfig.SetEnableMulticast
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IWMReaderNetworkConfig::SetEnableMulticast


## -description



The <b>SetEnableMulticast</b> method enables or disables multicasting.




## -parameters




### -param fEnableMulticast [in]

Boolean value that is True if multicasting is to be enabled.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

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
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
NULL or invalid argument passed in.

</td>
</tr>
</table>
 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nn-wmsdkidl-iwmreadernetworkconfig">IWMReaderNetworkConfig Interface</a>



<a href="https://docs.microsoft.com/windows/desktop/api/wmsdkidl/nf-wmsdkidl-iwmreadernetworkconfig-getenablemulticast">IWMReaderNetworkConfig::GetEnableMulticast</a>
 

 

