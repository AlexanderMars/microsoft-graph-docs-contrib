---
title: "onEmailOtpSendListener resource type"
description: "**Listener for the onEmailOtpSend event"
author: "AlexanderMars"
ms.localizationpriority: medium
ms.subservice: "entra-sign-in"
doc_type: resourcePageType
---

# onEmailOtpSendListener resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Used for configuring the applications to listen the onEmailOtpSend event, the corresponding custom extension handler ID, and the request timeout length.


Inherits from [authenticationEventListener](../resources/authenticationeventlistener.md).


## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List](../api/onemailotpsendlistener-list.md)|[onEmailOtpSendListener](../resources/onemailotpsendlistener.md) collection|Get a list of the [onEmailOtpSendListener](../resources/onemailotpsendlistener.md) objects and their properties.|
|[Get](../api/onemailotpsendlistener-get.md)|[onEmailOtpSendListener](../resources/onemailotpsendlistener.md)|Read the properties and relationships of an [onEmailOtpSendListener](../resources/onemailotpsendlistener.md) object.|
|[Update](../api/onemailotpsendlistener-update.md)|[onEmailOtpSendListener](../resources/onemailotpsendlistener.md)|Update the properties of an [onEmailOtpSendListener](../resources/onemailotpsendlistener.md) object.|
|[Delete](../api/onemailotpsendlistener-delete.md)|None|Delete an [onEmailOtpSendListener](../resources/onemailotpsendlistener.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|authenticationEventsFlowId|String|**TODO: Add Description** Inherited from [authenticationEventListener](../resources/authenticationeventlistener.md).|
|conditions|[authenticationConditions](../resources/authenticationconditions.md)|**TODO: Add Description** Inherited from [authenticationEventListener](../resources/authenticationeventlistener.md).|
|handler|[onOtpSendHandler](../resources/onotpsendhandler.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|priority|Int32|**TODO: Add Description** Inherited from [authenticationEventListener](../resources/authenticationeventlistener.md).|

## Relationships
None.

## JSON representation
The following JSON representation shows the resource type.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onEmailOtpSendListener",
  "baseType": "microsoft.graph.authenticationEventListener",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onEmailOtpSendListener",
  "id": "String (identifier)",
  "priority": "Integer",
  "conditions": {
    "@odata.type": "microsoft.graph.authenticationConditions"
  },
  "authenticationEventsFlowId": "String",
  "handler": {
    "@odata.type": "microsoft.graph.onOtpSendHandler"
  }
}
```

