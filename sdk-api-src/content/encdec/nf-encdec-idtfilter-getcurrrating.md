---
UID: NF:encdec.IDTFilter.GetCurrRating
title: IDTFilter::GetCurrRating (encdec.h)
description: The GetCurrRating method retrieves the current rating, based on the most recent media sample.
helpviewer_keywords: ["GetCurrRating","GetCurrRating method [Microsoft TV Technologies]","GetCurrRating method [Microsoft TV Technologies]","IDTFilter interface","IDTFilter interface [Microsoft TV Technologies]","GetCurrRating method","IDTFilter.GetCurrRating","IDTFilter::GetCurrRating","IDTFilterGetCurrRating","encdec/IDTFilter::GetCurrRating","mstv.idtfilter_getcurrrating"]
old-location: mstv\idtfilter_getcurrrating.htm
tech.root: mstv
ms.assetid: 6ea5c9a0-b04c-41a6-83ed-48ea9d187da7
ms.date: 12/05/2018
ms.keywords: GetCurrRating, GetCurrRating method [Microsoft TV Technologies], GetCurrRating method [Microsoft TV Technologies],IDTFilter interface, IDTFilter interface [Microsoft TV Technologies],GetCurrRating method, IDTFilter.GetCurrRating, IDTFilter::GetCurrRating, IDTFilterGetCurrRating, encdec/IDTFilter::GetCurrRating, mstv.idtfilter_getcurrrating
f1_keywords:
- encdec/IDTFilter.GetCurrRating
dev_langs:
- c++
req.header: encdec.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP1 [desktop apps only]
req.target-min-winversvr: None supported
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
- EncDec.h
api_name:
- IDTFilter.GetCurrRating
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDTFilter::GetCurrRating


## -description


The <b>GetCurrRating</b> method retrieves the current rating, based on the most recent media sample.


## -parameters




### -param pEnSystem [out]

Receives the rating system, as an <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tvratings/ne-tvratings-entvrat_system">EnTvRat_System</a> enumeration type.


### -param pEnRating [out]

Receives the rating level, as an <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tvratings/ne-tvratings-entvrat_genericlevel">EnTvRat_GenericLevel</a> enumeration type. The meaning of this value depends on the rating system.


### -param plbfEnAttr [out]

Receives a bitwise combination of flags from the <a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/tvratings/ne-tvratings-bfentvrat_genericattributes">BfEnTvRat_GenericAttributes</a> enumeration. The flags specify content attributes, such as violence or adult language. Content attributes do not apply to all rating systems.


## -returns



Returns S_OK if successful, or an error code otherwise.




## -see-also




<a href="https://docs.microsoft.com/previous-versions/windows/desktop/api/encdec/nn-encdec-idtfilter">IDTFilter Interface</a>
 

 

