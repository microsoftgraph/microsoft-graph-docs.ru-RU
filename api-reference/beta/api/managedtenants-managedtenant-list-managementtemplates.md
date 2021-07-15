---
title: Управление спискамиTemplates
description: Получите список объектов managementTemplate и их свойств.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 624e786738efbe2e89052e6321f02b838b7e5c1c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443071"
---
# <a name="list-managementtemplates"></a>Управление спискамиTemplates
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [managementTemplate](../resources/managedtenants-managementtemplate.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|ManagedTenants.Read.All, ManagedTenants.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managementTemplates
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов managementTemplate](../resources/managedtenants-managementtemplate.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_managementtemplate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managementTemplates
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-managementtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-managementtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-managementtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-managementtemplate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managementTemplate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/managementTemplates",
  "value": [
    {
      "id": "e5834405-43d2-4815-867d-3dd600308d1c_1",
      "displayName": "Baseline - Block Legacy Authentication",
      "description": null,
      "category": "identity",
      "parameters": [
        {
          "valueType": "string",
          "displayName": "DisplayName",
          "description": null,
          "jsonDefaultValue": "\"Baseline - Block Legacy Authentication\"",
          "jsonAllowedValues": "null"
        },
        {
          "valueType": "string",
          "displayName": "State",
          "description": null,
          "jsonDefaultValue": "\"enabledForReportingButNotEnforced\"",
          "jsonAllowedValues": "[\"enabled\",\"disabled\",\"enabledForReportingButNotEnforced\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "ClientAppTypes",
          "description": null,
          "jsonDefaultValue": "[\"exchangeActiveSync\",\"other\"]",
          "jsonAllowedValues": "[\"exchangeActiveSync\",\"other\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeApplications",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeUsers",
          "description": null,
          "jsonDefaultValue": "[\"None\"]",
          "jsonAllowedValues": "[\"All\",\"None\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "IncludeLocations",
          "description": null,
          "jsonDefaultValue": "[\"All\"]",
          "jsonAllowedValues": "[\"All\",\"AllTrusted\"]"
        },
        {
          "valueType": "string",
          "displayName": "GrantControls.Operator",
          "description": null,
          "jsonDefaultValue": "\"OR\"",
          "jsonAllowedValues": "[\"OR\",\"AND\"]"
        },
        {
          "valueType": "stringCollection",
          "displayName": "GrantControls.BuiltInControls",
          "description": null,
          "jsonDefaultValue": "[\"block\"]",
          "jsonAllowedValues": "[\"block\"]"
        }
      ],
      "workloadActions": [
        {
          "actionId": "6a3ad0bc-5d7e-4a49-a105-c559aa4633e1",
          "category": "automated",
          "displayName": "ConditionalAccessPolicy",
          "description": null,
          "service": "AAD",
          "settings": [
            {
              "valueType": "string",
              "displayName": "DisplayName",
              "overwriteAllowed": false,
              "jsonValue": "\"Baseline - Block Legacy Authentication\""
            },
            {
              "valueType": "string",
              "displayName": "State",
              "overwriteAllowed": false,
              "jsonValue": "\"enabledForReportingButNotEnforced\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "ClientAppTypes",
              "overwriteAllowed": false,
              "jsonValue": "[\"exchangeActiveSync\",\"other\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeApplications",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeUsers",
              "overwriteAllowed": false,
              "jsonValue": "[\"None\"]"
            },
            {
              "valueType": "stringCollection",
              "displayName": "IncludeLocations",
              "overwriteAllowed": false,
              "jsonValue": "[\"All\"]"
            },
            {
              "valueType": "string",
              "displayName": "GrantControls.Operator",
              "overwriteAllowed": false,
              "jsonValue": "\"OR\""
            },
            {
              "valueType": "stringCollection",
              "displayName": "GrantControls.BuiltInControls",
              "overwriteAllowed": false,
              "jsonValue": "[\"block\"]"
            }
          ]
        }
      ]
    }
  ]
}
```
