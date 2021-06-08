---
title: Удаление timeCard
description: Удаление экземпляра timeCard в расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f87fe8145d65793b33dc539ed1db235a7e09aebf
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787919"
---
# <a name="delete-timecard"></a>Удаление timeCard

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Удаление [экземпляра timeCard](../resources/timeCard.md) в [расписании.](../resources/schedule.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Schedule.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Schedule.ReadWrite.All* |

>\***Важно:** При использовании разрешений приложения необходимо включить в запрос `MS-APP-ACTS-AS` заготвую.

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timecards/{timeCardID}
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| MS-APP-ACTS-AS | ID пользователя, от имени которого действует приложение. Требуется при использовании области разрешений приложения. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса. 

<!-- {
  "blockType": "request",
  "name": "timecard-delete"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule/timecards/3895809b-a618-4c0d-86a0-d42b25b7d74f
```

### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete timeCard",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
