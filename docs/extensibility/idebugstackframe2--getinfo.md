---
title: "IDebugStackFrame2::GetInfo"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: na
ms.topic: "article"
f1_keywords: 
  - "IDebugStackFrame2::GetInfo"
helpviewer_keywords: 
  - "IDebugStackFrame2::GetInfo"
ms.assetid: 19c6870b-b94e-453c-bf19-82ce95b79d26
caps.latest.revision: 10
ms.author: "gregvanl"
manager: "ghogen"
translation.priority.mt: 
  - "cs-cz"
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "pl-pl"
  - "pt-br"
  - "ru-ru"
  - "tr-tr"
  - "zh-cn"
  - "zh-tw"
---
# IDebugStackFrame2::GetInfo
Gets a description of the stack frame.  
  
## Syntax  
  
```cpp#  
HRESULT GetInfo (   
   FRAMEINFO_FLAGS dwFieldSpec,  
   UINT            nRadix,  
   FRAMEINFO*      pFrameInfo  
);  
```  
  
```c#  
int GetInfo (   
   enum_FRAMEINFO_FLAGS dwFieldSpec,  
   uint                 nRadix,  
   FRAMEINFO[]          pFrameInfo  
);  
```  
  
#### Parameters  
 `dwFieldSpec`  
 [in] A combination of flags from the [FRAMEINFO_FLAGS](../extensibility/frameinfo_flags.md) enumeration that specifies which fields of the `pFrameInfo` parameter are to be filled in.  
  
 `nRadix`  
 [in] The radix to be used in formatting any numerical information.  
  
 `pFrameInfo`  
 [out] A [FRAMEINFO](../extensibility/frameinfo.md) structure that is filled in with the description of the stack frame.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## See Also  
 [IDebugStackFrame2](../extensibility/idebugstackframe2.md)   
 [FRAMEINFO_FLAGS](../extensibility/frameinfo_flags.md)   
 [FRAMEINFO](../extensibility/frameinfo.md)