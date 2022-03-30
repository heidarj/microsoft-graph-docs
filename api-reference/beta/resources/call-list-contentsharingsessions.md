---
title: "List contentSharingSessions"
description: "Retrieve a list of contentSharingSession objects in the call."
author: "satyakonmsft"
ms.localizationpriority: medium
ms.prod: "cloud-communications"
doc_type: apiPageType
---

# List contentSharingSessions

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve a list of contentSharingSession objects in the call.

## Permissions

| Permission type | Permissions (from least to most privileged) |
| :-------------- | :------------------------------------------ |
| Delegated (work or school account)     | Not Supported        |
| Delegated (personal Microsoft account) | Not Supported        |
| Application     | None                                        |

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
GET /communications/calls/{id}/contentSharingSessions
```

## Request headers

| Name          | Description               |
|:--------------|:--------------------------|
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and collection of [contentSharingSession](../resources/contentsharingsession.md) objects in the response body.

## Example

### Request

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-contentsharingsessions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/contentSharingSessions
```
---

<!-- markdownlint-disable MD024 -->

### Response

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.contentSharingSession",
  "isCollection": true,
  "truncated": true
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "value":[
      {
         "@odata.type":"#microsoft.graph.contentSharingSession",
         "id":"a7ebfb2d-871e-419c-87af-27290b22e8db"
      },
      {
         "@odata.type":"#microsoft.graph.contentSharingSession",
         "id":"278405a3-f568-4b3e-b684-009193463064"
      }
   ],
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/contentSharingSessions"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List contentSharingSessions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

