---
title: Перечисление directoryAudits
description: Описывает метод List ресурса Директоряудит (Entity) из API Microsoft Graph.
localization_priority: Normal
author: SarahBar
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a06d02929ca194d29820cedbe4b40aea5590035
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601610"
---
# <a name="list-directoryaudits"></a>Перечисление directoryAudits

Пространство имен: microsoft.graph

Получение списка журналов аудита, созданных Azure Active Directory. К ним относятся журналы аудита, созданные различными службами в Azure AD, в том числе Управление пользователями, приложениями, устройствами и группами, управление правами на доступ к данным, проверки доступа, условия использования, защиту учетных записей, управление паролями (сброс паролей самообслуживания и администратора) и самостоятельное управление группами и т. д.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Аудитлог. Read. ALL и Directory. Read. ALL    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается                               |
| Для приложений                            | AuditLog.Read.All                           |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryaudits
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает следующие параметры запроса OData для настройки ответа. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query_parameters).

| Параметр                                                       | Описание                                                                   | Пример                                                                     |
| :--------------------------------------------------------- | :---------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [\$Фишинг](/graph/query_parameters#filter-parameter)       | Фильтрует результаты (строки).                                                       | `/auditLogs/directoryAudits?&$filter=activityDateTime le 2018-01-24`         |
| [\$Вверх](/graph/query_parameters#top-parameter)             | Задает размер страницы результатов.                                                | `/auditLogs/directoryAudits?$top=1`                                         |
| [\$skiptoken](/graph/query_parameters#skiptoken-parameter) | Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. | `/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a>Атрибуты, поддерживаемые \$ параметром Filter

| Атрибут                                                    | Поддерживаемые операторы |
| :----------------------------------------------------------- | :------------------ |
| activityDisplayName                                          | eq, startswith      |
| activityDateTime                                             | eq, ge, le          |
| loggedByService                                              | eq                  |
| initiatedBy/user/id                                          | eq                  |
| initiatedBy/user/displayName                                 | eq                  |
| initiatedBy/user/userPrincipalName                           | eq, startswith      |
| initiatedBy/app/appId                                        | eq                  |
| Инитиатедби/App/displayName                                  | eq                  |
| Таржетресаурцес/Any (t: t/ID EQ ' {значение} ')                    | eq                  |
| Таржетресаурцес/Any (t: t/displayName EQ ' {значение} ')            | eq                  |
| Таржетресаурцес/Any (x: StartsWith (x/displayName, ' {значение} ')) | startswith          |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
| :------------ | :------------ |
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [директоряудит](../resources/directoryaudit.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryaudit",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```

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
        "targetResources": [{
            "id": "ef7e527d-6c92-4234-8c6d-cf6fdfb57f95",
            "displayName": "Example.com",
            "Type": "Group",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"}],
            "groupType": "unifiedGroups"
            }, 
            {
            "id": "1f0e98f5-3161-4c6b-9b50-d488572f2bb7",
            "displayName": null,
            "Type": "User",
            "modifiedProperties": [],
            "userPrincipalName": "bob@contoso.com"
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
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

