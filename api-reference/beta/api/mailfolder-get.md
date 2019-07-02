---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33932d16ac51f385a66adfd6fd8010069b650bf2
ms.sourcegitcommit: ee710ff556f4a7907181df5c323e345f52808ce2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35417740"
---
# <a name="get-mailfolder"></a>Получение объекта mailFolder

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение свойств и связей объекта папки сообщений.

Существует два сценария, в которых приложение может получить папку почты другого пользователя:

* У приложения есть разрешения для приложений; или
* У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ. См. [подробные сведения и пример](/graph/outlook-share-messages-folders).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Mail. ReadBasic, mail. Read, mail. ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Mail. ReadBasic, mail. Read, mail. ReadWrite    |
|Для приложений | Mail.Read, Mail.ReadWrite |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Тип   | Описание               |
|:--------------|:-------|:--------------------------|
| Authorization | string | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-a-mail-folder"></a>Пример 1: получение почтовой папки

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGVmMDEzM",
  "displayName": "Inbox",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 2,
  "unreadItemCount": 59,
  "totalItemCount": 60,
  "wellKnownName": "inbox"
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-get-a-mail-search-folder"></a>Пример 2: Получение папки поиска почты

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGVmMDEzM"],
  "name": "get_mailSearchfolder"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzN
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "AAMkAGVmMDEzN",
  "displayName": "Get MyAnalytics",
  "parentFolderId": "AAMkAGVmMDEzI",
  "childFolderCount": 0,
  "unreadItemCount": 6,
  "totalItemCount": 6,
  "wellKnownName": null,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "AAMkAGVmMDEzM"
  ],
  "filterQuery": "contains(subject, 'MyAnalytics')"
}
```
#### <a name="sdk-sample-code"></a>Пример кода SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Цель — C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_mailSearchfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
