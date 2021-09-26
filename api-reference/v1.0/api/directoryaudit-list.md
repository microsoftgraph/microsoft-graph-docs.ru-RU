---
title: Перечисление directoryAudits
description: Описывает метод списка ресурса directoryAudit (сущности) из API Microsoft Graph.
ms.localizationpriority: medium
author: SarahBar
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 4ce9c6c23b474c9100b66f463e790bccf0240887
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765818"
---
# <a name="list-directoryaudits"></a>Перечисление directoryAudits

Пространство имен: microsoft.graph

Получите список журналов аудита, созданных Azure Active Directory. Это включает журналы аудита, созданные различными службами в Azure AD, в том числе пользователем, приложением, управлением устройствами и группой, привилегированным управлением удостоверениями (PIM), обзоры доступа, условия использования, защита удостоверений, управление паролями (сбросы паролей самообслуживающего и администратора), управление группой самообслуживаний и т. д.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | AuditLog.Read.All и Directory.Read.All    |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.                              |
| Application                            | AuditLog.Read.All и Directory.Read.All    |

> [!IMPORTANT]
> Этот API имеет [известные](/graph/known-issues#azure-ad-activity-reports) проблемы и в настоящее время требует согласия на оба **auditLog.Read.All** и **Directory.Read.All** разрешений.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /auditLogs/directoryaudits
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает следующие параметры запроса OData, чтобы помочь настроить ответ. Сведения об использовании этих параметров см. в статье [Параметры запросов OData](/graph/query-parameters).

| Параметр                                                       | Описание                                                                   | Пример                                                                     |
| :--------------------------------------------------------- | :---------------------------------------------------------------------------- | :-------------------------------------------------------------------------- |
| [\$фильтр](/graph/query-parameters#filter-parameter)       | Фильтрует результаты (строки).                                                       | `/auditLogs/directoryAudits?&$filter=activityDateTime le 2018-01-24`         |
| [\$Вверх](/graph/query-parameters#top-parameter)             | Задает размер страницы результатов.                                                | `/auditLogs/directoryAudits?$top=1`                                         |
| [\$skiptoken](/graph/query-parameters#skiptoken-parameter) | Возвращает следующую страницу результатов из результирующих наборов, занимающих несколько страниц. | `/auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1` |

### <a name="attributes-supported-by-filter-parameter"></a>Атрибуты, поддерживаемые \$ параметром фильтра

| Атрибут                                                    | Поддерживаемые операторы |
| :----------------------------------------------------------- | :------------------ |
| activityDisplayName                                          | eq, startswith      |
| activityDateTime                                             | eq, ge, le          |
| loggedByService                                              | eq                  |
| initiatedBy/user/id                                          | eq                  |
| initiatedBy/user/displayName                                 | eq                  |
| initiatedBy/user/userPrincipalName                           | eq, startswith      |
| initiatedBy/app/appId                                        | eq                  |
| initiatedBy/app/displayName                                  | eq                  |
| targetResources/any(t: t/id eq '{value}')                    | eq                  |
| targetResources/any (t:t/displayName eq '{value}')            | eq                  |
| targetResources/any(x: startswith(x/displayName, '{value}'))) | startswith          |

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
| :------------ | :------------ |
| Авторизация | Bearer {code} |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [directoryAudit](../resources/directoryaudit.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directoryaudit_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directoryaudit-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directoryaudit-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directoryaudit-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directoryaudit-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271

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

