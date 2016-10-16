---
title: "XML documentation parse error: Start tag &#39;&lt;tag&gt;&#39; doesn&#39;t have a matching end tag"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 45b68176-ebf6-43af-820e-6801aabb6c57
caps.latest.revision: 11
manager: douge
translation.priority.ht: 
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - ru-ru
  - zh-cn
  - zh-tw
translation.priority.mt: 
  - cs-cz
  - pl-pl
  - pt-br
  - tr-tr
---
# XML documentation parse error: Start tag &#39;&lt;tag&gt;&#39; doesn&#39;t have a matching end tag
XML documentation parse error: Start tag <tag\> doesn't have a matching end tag. XML comment will be ignored.  
  
 The XML comment contains a start tag but does not contain a matching end tag.  
  
 **Error ID:** BC42316  
  
### To correct this error  
  
-   Add an end tag that matches the start tag.  
  
     — or —  
  
-   If the tag contains no inner text, such as [<seealso\>](../Topic/%3Cseealso%3E%20\(Visual%20Basic\).md), specify a forward slash before the closing angle bracket.  
  
## See Also  
 [XML Comment Tags](../Topic/Recommended%20XML%20Tags%20for%20Documentation%20Comments%20\(Visual%20Basic\).md)   
 [Documenting Your Code with XML](../Topic/Documenting%20Your%20Code%20with%20XML%20\(Visual%20Basic\).md)