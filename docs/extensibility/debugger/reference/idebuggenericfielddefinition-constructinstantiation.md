---
title: "IDebugGenericFieldDefinition::ConstructInstantiation | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-sdk"
ms.tgt_pltfrm: ""
ms.topic: "article"
helpviewer_keywords: 
  - "ConstructInstantiation"
  - "IDebugGenericFieldDefinition::ConstructInstantiation"
ms.assetid: ef8ae261-a98b-4dc2-93b3-7c5191818ba2
caps.latest.revision: 8
author: "gregvanl"
ms.author: "gregvanl"
manager: ghogen
---
# IDebugGenericFieldDefinition::ConstructInstantiation
Constructs a field instance given an array of type arguments.  
  
## Syntax  
  
```cpp  
HRESULT ConstructInstantiation(  
   ULONG32       cArgs,  
   IDebugField** ppArgs,  
   IDebugField** ppConstructedField  
);  
```  
  
```csharp  
int ConstructInstantiation(  
   uint            cArgs,  
   IDebugField[]   ppArgs,  
   out IDebugField ppConstructedField  
);  
```  
  
#### Parameters  
 `cArgs`  
 [in] Number of arguments in the `ppArgs` array.  
  
 `ppArgs`  
 [in] Array that contains the type arguments. The type arguments must be closed types (non-generic or fully instantiated generics).  
  
 `ppConstructedField`  
 [out] Returns the [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) interface that represents the new field.  
  
## Return Value  
 If successful, returns `S_OK`; otherwise, returns an error code.  
  
## Remarks  
 Constraints are not checked.  
  
## See Also  
 [IDebugGenericFieldDefinition](../../../extensibility/debugger/reference/idebuggenericfielddefinition.md)