---
title: Получение directoryAudit
description: Описывает метод Get ресурса Директоряудит (Entity) из API Microsoft Graph.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 214a1979ed1bfdecca00f62dd506c68ebc36370a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275616"
---
# <a name="get-directoryaudit"></a>Получение directoryAudit

Получение конкретного элемента журнала аудита Azure Active Directory. Сюда входит элемент журнала аудита, созданный различными службами в Azure Active Directory, такими как пользователь, приложение, Управление устройствами и группами, управление правами на доступ к данным, обзоры доступа, условия использования, защита удостоверений, управление паролями ( самообслуживания и сброс паролей администратора), самостоятельное управление группами и т. д.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Аудитлог. Read. ALL и Directory. Read. ALL |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается   |
|Для приложений | AuditLog.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметры запросов OData для настройки ответа. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [директоряудит](../resources/directoryaudit.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->

```http
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits/{id}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.
>**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryaudit"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 218
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directoryaudit-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directoryaudit-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directoryaudit-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#auditlogs/directoryaudits",
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "728309ae-1a37-4937-9afe-e35d964db09b",
                "displayName": "Audry Oliver",
                "userPrincipalName": "bob@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResource": [{
            "id": "ef7e527d-6c92-4234-8c6d-cf6fdfb57f95",
            "displayName": "Example.com",
            "Type": "Group",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync" }],
            "groupType": "unifiedGroups"
            }],
        }, {
            "id": "1f0e98f5-3161-4c6b-9b50-d488572f2bb7",
            "displayName": null,
            "Type": "User",
            "modifiedProperties": [],
            "userPrincipalName": "example@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryaudit-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryaudit-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryaudit-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
