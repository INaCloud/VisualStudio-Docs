---
title: "Compiler Warning (level 3) CS0419"
ms.custom: na
ms.date: 10/02/2016
ms.devlang: 
  - CSharp
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-csharp
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: de439ad5-422f-4ed6-96d6-69dade29c7b2
caps.latest.revision: 8
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
# Compiler Warning (level 3) CS0419
Ambiguous reference in cref attribute: 'Method Name1'.  Assuming 'Method Name2', but could have also matched other overloads including 'Method Name3'.  
  
 In an XML documentation comment in the code, a reference could not be resolved. This could occur if the method is overloaded, or if two different identifiers with the same name are found. To resolve the warning, use a qualified name to disambiguate the reference, or include the specific overload in parentheses.  
  
 The following sample generates CS0419.  
  
```  
// cs0419.cs  
// compile with: /doc:x.xml /W:3  
interface I  
{  
   /// text for F(void)  
   void F();  
   /// text for F(int)  
   void F(int i);  
}  
/// text for class MyClass  
public class MyClass  
{  
   /// <see cref="I.F"/>  
   public static void MyMethod(int i)  
   {  
   }  
/* Try this instead:  
   /// <see cref="I.F(int)"/>  
   public static void MyMethod(int i)  
   {  
   }  
*/  
   /// text for Main  
   public static void Main ()  
   {  
   }  
}  
```