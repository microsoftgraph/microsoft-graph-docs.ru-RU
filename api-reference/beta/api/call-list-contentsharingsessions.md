---
title: Перечисление contentSharingSessions
description: Получение списка объектов contentSharingSession в вызове.
author: satyakonmsft
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b7fdbb45f2eb25e0be5fb55f0417fd602290cb64
ms.sourcegitcommit: 9bbcce5784a89768ece55a66e3651080d56e1e92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/19/2022
ms.locfileid: "64917967"
---
# <a name="list-contentsharingsessions"></a>Перечисление contentSharingSessions

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [contentSharingSession](../resources/contentsharingsession.md) в вызове.

## <a name="permissions"></a>Разрешения

| Тип разрешения | Разрешения (в порядке повышения привилегий) |
| :-------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Не поддерживается.       |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается.       |
| Application     | Calls.JoinGroupCallAsGuest.All, Calls.JoinGroupCall.All, Calls.Initiate.All, Calls.InitiateGroupCall.All                                        |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /communications/calls/{id}/contentSharingSessions
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
|:--------------|:--------------------------|
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [contentSharingSession](../resources/contentsharingsession.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get-contentsharingsessions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/7531d31f-d10d-44de-802f-c569dbca451c/contentSharingSessions
```

<!-- markdownlint-disable MD024 -->

### <a name="response"></a>Отклик

Ниже приведен пример ответа.

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
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#communications/calls('7531d31f-d10d-44de-802f-c569dbca451c')/contentSharingSessions"
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
