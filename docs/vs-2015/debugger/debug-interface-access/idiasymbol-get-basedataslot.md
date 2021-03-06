---
title: "IDiaSymbol::get_baseDataSlot | Microsoft Docs"
ms.custom: ""
ms.date: "2018-06-30"
ms.prod: "visual-studio-dev14"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-debug"
ms.tgt_pltfrm: ""
ms.topic: "article"
dev_langs: 
  - "C++"
ms.assetid: f9ed21b7-9397-4813-926e-ade11914b06b
caps.latest.revision: 6
author: "mikejo5000"
ms.author: "mikejo"
manager: "ghogen"
---
# IDiaSymbol::get_baseDataSlot
[!INCLUDE[vs2017banner](../../includes/vs2017banner.md)]

The latest version of this topic can be found at [IDiaSymbol::get_baseDataSlot](https://docs.microsoft.com/visualstudio/debugger/debug-interface-access/idiasymbol-get-basedataslot).  
  
Retrieves the base data slot.  
  
## Syntax  
  
```cpp  
HRESULT get_baseDataSlot(   
   DWORD* pRetVal);  
```  
  
#### Parameters  
 `pRetVal`  
 [out] A pointer to a `DWORD` that holds the base data slot.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.  
  
## See Also  
 [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)



