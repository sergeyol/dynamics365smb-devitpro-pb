---
title: "TestRequestPage.Next() Method"
description: "Sets the current row of the test page as the next row in the data set."
ms.author: solsen
ms.custom: na
ms.date: 07/07/2021
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: reference
ms.service: "dynamics365-business-central"
author: SusanneWindfeldPedersen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# TestRequestPage.Next() Method
> **Version**: _Available or changed with runtime version 1.0._

Sets the current row of the test page as the next row in the data set.


## Syntax
```AL
[Ok := ]  TestRequestPage.Next()
```

## Parameters
*TestRequestPage*  
&emsp;Type: [TestRequestPage](testrequestpage-data-type.md)  
An instance of the [TestRequestPage](testrequestpage-data-type.md) data type.  

## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the current row has changed, otherwise **false**. Throws a NavTestPageNotOpenedException if the page is not opened.
      


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[TestRequestPage Data Type](testrequestpage-data-type.md)  
[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)