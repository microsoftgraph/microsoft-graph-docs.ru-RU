---
title: Список Унифиедроледефинитионс
description: Получение списка объектов Унифиедроледефинитион.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a0d8ed68ea3e4f8027e44409246ea56b45557bb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019777"
---
# <a name="list-unifiedroledefinitions"></a>Список Унифиедроледефинитионс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [унифиедроледефинитион](../resources/unifiedroledefinition.md) для поставщика.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL, Directory. AccessAsUser. ALL    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Для приложений | Ролеманажемент. Read. Directory, Directory. Read. ALL, Ролеманажемент. ReadWrite. Directory, Directory. ReadWrite. ALL |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /roleManagement/directory/roleDefinitions
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает `$filter` `id` , `displayName` и `isBuiltIn` . Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization | Bearer {token} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [унифиедроледефинитион](../resources/unifiedroledefinition.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roledefinitions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roledefinitions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roledefinitions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roledefinitions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleDefinition",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions",
    "value": [
        {
            "id": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "description": "Can reset passwords for non-administrators and Helpdesk Administrators.",
            "displayName": "Helpdesk Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/users/invalidateAllRefreshTokens",
                        "microsoft.directory/users/bitLockerRecoveryKeys/read",
                        "microsoft.directory/users/password/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('729827e3-9c14-49f7-bb1b-9608f156bbb8')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "f023fd81-a637-4b56-95fd-791ac0226033",
            "description": "Can read service health information and manage support tickets.",
            "displayName": "Service Support Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "f023fd81-a637-4b56-95fd-791ac0226033",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('f023fd81-a637-4b56-95fd-791ac0226033')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        },
        {
            "id": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "description": "Can perform common billing related tasks like updating payment information.",
            "displayName": "Billing Administrator",
            "isBuiltIn": true,
            "isEnabled": true,
            "templateId": "b0f54661-2d74-4c50-afa3-1ec803f12efe",
            "version": "1",
            "rolePermissions": [
                {
                    "allowedResourceActions": [
                        "microsoft.directory/organization/basic/update",
                        "microsoft.azure.serviceHealth/allEntities/allTasks",
                        "microsoft.azure.supportTickets/allEntities/allTasks",
                        "microsoft.commerce.billing/allEntities/allTasks",
                        "microsoft.office365.webPortal/allEntities/standard/read",
                        "microsoft.office365.serviceHealth/allEntities/allTasks",
                        "microsoft.office365.supportTickets/allEntities/allTasks"
                    ],
                    "condition": null
                }
            ],
            "inheritsPermissionsFrom@odata.context": "https://graph.microsoft.com/beta/$metadata#roleManagement/directory/roleDefinitions('b0f54661-2d74-4c50-afa3-1ec803f12efe')/inheritsPermissionsFrom",
            "inheritsPermissionsFrom": [
                {
                    "id": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
                }
            ]
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List roleDefinitions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


