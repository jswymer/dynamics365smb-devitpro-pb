---
title: customer resource type (Beta)
description: A customer object in Dynamics 365 Business Central (Beta).
author: SusanneWindfeldPedersen
ms.topic: reference
ms.devlang: al
ms.date: 05/31/2024
ms.author: solsen
ms.reviewer: solsen
---

# customer resource type (Beta)

<!-- START>DO_NOT_EDIT -->
<!-- IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT. -->
Represents a customer in [!INCLUDE[prod_short](../../../includes/prod_short.md)].

> [!NOTE]
> For information about enabling APIs for [!INCLUDE[prod_short](../../../includes/prod_short.md)] see [Enabling the APIs for Dynamics 365 Business Central](../../../api-reference/v2.0/enabling-apis-for-dynamics-nav.md).

## Methods

| Method | Return Type|Description |
|:--------------------|:-----------|:-------------------------|
|[GET customer](../api/dynamics_customer_get.md)|customer|Gets a customer object.|



## Properties

| Property           | Type   |Description     |
|:-------------------|:-------|:---------------|
|id|GUID|The unique ID of the customer. Non-editable.|
|number|string|Specifies the number of the customer.|
|displayName|string|Specifies the customer's name. This name will appear on all sales documents for the customer.|
|type|string||
|city|string|Specifies the customer's city.|
|state|string|Specifies the customer's state.|
|country|string|Specifies the customer's country.|
|postalCode|string|Specifies the customer's postal code.|
|salespersonCode|string||
|balanceDue|decimal|Specifies total balance due.|
|creditLimit|decimal||
|currencyCode|string|The default currency code for the customer.|
|blocked|string|Specifies that transactions with the customer cannot be posted. Set to **All**, if the customer is blocked, set to blank if not blocked.|
|lastModifiedDateTime|datetime|The last datetime the customer was modified. Read-Only.|

## JSON representation

Here is a JSON representation of the customer resource.


```json
{
    "id": "GUID",
    "number": "string",
    "displayName": "string",
    "type": "string",
    "city": "string",
    "state": "string",
    "country": "string",
    "postalCode": "string",
    "salespersonCode": "string",
    "balanceDue": "decimal",
    "creditLimit": "decimal",
    "currencyCode": "string",
    "blocked": "string",
    "lastModifiedDateTime": "datetime"
}
```
<!-- IMPORTANT: END>DO_NOT_EDIT -->

## Related information
[GET customer](../api/dynamics_customer_get.md)
