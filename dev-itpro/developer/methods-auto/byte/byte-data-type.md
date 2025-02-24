---
title: "Byte Data Type"
description: "Stores a single, 8-bit character as a value in the range 0 to 255."
ms.author: solsen
ms.custom: na
ms.date: 06/23/2021
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
# Byte Data Type
> **Version**: _Available or changed with runtime version 1.0._

Stores a single, 8-bit character as a value in the range 0 to 255. You can easily convert this data type from a number to a character and vice versa. This means you can use mathematical operators on Byte variables.




[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Example

The following example assumes that you have a Byte variable named B and a Text variable named S.  
  
You can assign a constant string of the length 1 to a Byte variable, as shown in the first line of the following code example. You can assign a single character in a Text or Code variable to a Byte variable, as shown in the second line of the following code example. You can assign a numeric value to a Byte variable, as shown in the third line of the following code example. This causes the Byte variable to contain the character from the ASCII character set that corresponds to the numeric ASCII code.  
  
```al
B := 'A';  
B := S[2];  
B := 65;  
```  
  
You cannot assign a character to a position greater than the position of the null terminator. For example, if the value of the text variable *MyText* is 'abc', then the null terminator is at position 4 and the following assignment causes a run-time error to occur.  
  
```al
MyText[5] := 'e';  
```  
  
## See Also

[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)  