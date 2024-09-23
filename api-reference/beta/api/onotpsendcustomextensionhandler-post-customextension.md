---
title: "Create onOtpSendCustomExtension"
description: "Create a new onOtpSendCustomExtension object."
author: "AlexanderMars"
ms.localizationpriority: medium
ms.subservice: "entra-sign-in"
doc_type: apiPageType
---

# Create onOtpSendCustomExtension

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [onOtpSendCustomExtension](../resources/onotpsendcustomextension.md) object.

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- {
  "blockType": "permissions",
  "name": "onotpsendcustomextensionhandler-post-customextension-permissions"
}
-->
[!INCLUDE [permissions-table](../includes/permissions/onotpsendcustomextensionhandler-post-customextension-permissions.md)]

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.onOtpSendCustomExtension not found
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required. Learn more about [authentication and authorization](/graph/auth/auth-concepts).|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the [onOtpSendCustomExtension](../resources/onotpsendcustomextension.md) object.

You can specify the following properties when creating an **onOtpSendCustomExtension**.

**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|authenticationConfiguration|[customExtensionAuthenticationConfiguration](../resources/customextensionauthenticationconfiguration.md)|**TODO: Add Description** Inherited from [customCalloutExtension](../resources/customcalloutextension.md). Optional.|
|clientConfiguration|[customExtensionClientConfiguration](../resources/customextensionclientconfiguration.md)|**TODO: Add Description** Inherited from [customCalloutExtension](../resources/customcalloutextension.md). Optional.|
|description|String|**TODO: Add Description** Inherited from [customCalloutExtension](../resources/customcalloutextension.md). Optional.|
|displayName|String|**TODO: Add Description** Inherited from [customCalloutExtension](../resources/customcalloutextension.md). Optional.|
|endpointConfiguration|[customExtensionEndpointConfiguration](../resources/customextensionendpointconfiguration.md)|**TODO: Add Description** Inherited from [customCalloutExtension](../resources/customcalloutextension.md). Optional.|



## Response

If successful, this method returns a `201 Created` response code and an [onOtpSendCustomExtension](../resources/onotpsendcustomextension.md) object in the response body.

## Examples

### Request

The following example shows a request.
<!-- {
  "blockType": "request",
  "name": "create_onotpsendcustomextension_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.onOtpSendCustomExtension not found
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onOtpSendCustomExtension",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  },
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "description": "String",
  "displayName": "String",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  }
}
```


### Response

The following example shows the response.
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onOtpSendCustomExtension"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onOtpSendCustomExtension",
  "id": "1c8b03b2-7663-fbe9-960a-bc541decd469",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionAuthenticationConfiguration"
  },
  "clientConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionClientConfiguration"
  },
  "description": "String",
  "displayName": "String",
  "endpointConfiguration": {
    "@odata.type": "microsoft.graph.customExtensionEndpointConfiguration"
  }
}
```

