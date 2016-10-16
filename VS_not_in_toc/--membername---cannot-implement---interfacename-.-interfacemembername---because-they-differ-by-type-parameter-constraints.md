---
title: "&#39;&lt;membername&gt;&#39; cannot implement &#39;&lt;interfacename&gt;.&lt;interfacemembername&gt;&#39; because they differ by type parameter constraints"
ms.custom: na
ms.date: 10/01/2016
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: 2c971345-edb4-491e-9202-8eb8286b66f8
caps.latest.revision: 10
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
# &#39;&lt;membername&gt;&#39; cannot implement &#39;&lt;interfacename&gt;.&lt;interfacemembername&gt;&#39; because they differ by type parameter constraints
A generic event, property, or procedure attempts to implement a similar member defined in an interface, but they have different constraint lists on their type parameters.  
  
 To implement an interface member, the implementing member must match not only the complete signature of the interface member, but also the passing mechanism of each parameter.  
  
 To implement a generic interface member, the implementing member must additionally match the number of type parameters and the constraint list of each one.  
  
 For details on interface implementation, see [NOT IN BUILD: Implements Keyword and Implements Statement](assetId:///b96560f7-6413-480f-a1e2-f80253bab5be).  
  
 **Error ID:** BC32078  
  
### To correct this error  
  
-   If you intend to implement the interface member, revise the type parameter constraints to exactly match those of the interface member.  
  
-   If the type parameter constraints must remain as you have them, you cannot implement the interface member in this declaration. Remove the [Implements](../Topic/Implements%20Clause%20\(Visual%20Basic\).md) keyword from the declaration.  
  
## See Also  
 [Generic Types in Visual Basic](../Topic/Generic%20Types%20in%20Visual%20Basic%20\(Visual%20Basic\).md)   
 [NOT IN BUILD: Interface Implementation Examples in Visual Basic](assetId:///50bf2a30-73b6-4126-a921-075fd6eec278)