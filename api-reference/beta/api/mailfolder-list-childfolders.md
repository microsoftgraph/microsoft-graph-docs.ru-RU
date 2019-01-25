---
title: Список childFolders
description: 'Получите коллекцию папок в указанной папке. Можно использовать `.../me/MailFolders` ярлык для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 9d54828b97bb82c9ce0ee9eceeee86a4aa975c3d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512551"
---
# <a name="list-childfolders"></a>Список childFolders

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail.Read, Mail.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Mail.Read, Mail.ReadWrite    |
|Для приложений | Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Тип | Описание|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.

## <a name="example-1"></a>Пример 1
#### <a name="request-1"></a>Запрос 1
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a>Отклик 1
Ниже приведен пример отклика.
>**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

## <a name="example-2"></a>Пример 2
#### <a name="request-2"></a>Запрос 2
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a>Ответ 2
Ниже приведен пример ответа.
>**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
        "id": "AAMkAGVmMDEzA",
        "displayName": "Internal Screens",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 2,
        "totalItemCount": 2,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzB",
        "displayName": "Project Falcon",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 0,
        "unreadItemCount": 5,
        "totalItemCount": 5,
        "wellKnownName": null
    },
    {
        "id": "AAMkAGVmMDEzMA",
        "displayName": "Finder",
        "parentFolderId": "AAMkAGVmMDEzM",
        "childFolderCount": 4,
        "unreadItemCount": 0,
        "totalItemCount": 0,
        "wellKnownName": "searchfolders"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
