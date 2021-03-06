---
title: "How to: Create an XML Schema from an XML Document | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-general"
ms.tgt_pltfrm: ""
ms.topic: "article"
ms.assetid: 1d6700a9-fd67-4794-8997-399589e99bec
caps.latest.revision: 2
author: "gewarren"
ms.author: "gewarren"
manager: ghogen
---
# How to: Create an XML Schema from an XML Document
The XML Editor allows you to create an XML Schema definition language (XSD) schema from an XML document. The XML instance document determines how the schema is generated in the following manner:  
  
-   If the XML document has no schema or Document Type Definition (DTD) associated with it, the data in the XML document is used to infer a new XML Schema.  
  
-   If the XML document contains an associated DTD, the external DTD and internal subset are converted to a corresponding XML Schema.  
  
-   If the XML document contains an inline XML-Data Reduced (XDR) schema, the XDR schema is converted to a corresponding XML Schema.  
  
The schemas that are created are then used to provide IntelliSense for the XML document.  
  
For more information about the schema inference engine, see [Inferring an XML Schema](/dotnet/standard/data/xml/inferring-an-xml-schema).  
  
### To create an XML Schema  
  
1.  Load an XML instance document into the XML Editor.  
  
2.  Click the **Create Schema** button from the **Toolbar**.  
  
     An XML Schema document is created and opened for each namespace found in the XML instance document. Each schema is opened as a temporary miscellaneous file.  
  
     The schemas can be saved to disk, added to your project, or discarded.  
  
    > [!NOTE]
    >  The **Create Schema** command is also available from the shortcut menu of the XML Editor and under the **XML** menu.  
  
## See Also  
 [XML Editor](../xml-tools/xml-editor.md)