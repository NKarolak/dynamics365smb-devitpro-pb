---
title: "FilterPageHandler Attribute"
ms.custom: na
ms.date: 04/01/2020
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.service: "dynamics365-business-central"
author: jswymer
---

# FilterPageHandler Attribute

Specifies that the method is a FilterPageHandler method.

## Applies to  
 AL test methods on test codeunits. A test method is a method that has the [Test Attribute](devenv-test-attribute.md) declared. 

## Syntax  
  
```  
[FilterPageHandler]
FilterPageHandler(var RecRef: RecordRef) : Boolean;
```    

## Remarks

The **FilterPageHandler** method is called when a filter page is invoked in the code. It tests the UI that is generated by a **FilterPageBuilder** data type. 

The **FilterPageHandler** attribute requires that the method where it is applied has the signature `FilterPageHandler(var RecRef: RecordRef) : Boolean;`. The parameter variable, *RecRef*, holds the record of the filter page.

## See Also  
[Method Attributes](devenv-method-attributes.md)  
[Test Codeunits and Test Functions](../devenv-test-codeunits-and-test-methods.md)