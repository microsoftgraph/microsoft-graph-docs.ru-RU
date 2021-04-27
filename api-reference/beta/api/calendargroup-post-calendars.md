---
title: Создание объекта Calendar
description: С помощью этого API можно для экземпляра user создать календарь в группе календарей.
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f0f3fac9b9dcccb41ebea46b689080cfce879f4f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047702"
---
# <a name="create-calendar"></a>Создание объекта Calendar

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

С помощью этого API можно для экземпляра [user](../resources/user.md) создать календарь в группе календарей.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
| :------------------------------------- | :------------------------------------------ |
| Делегированные (рабочая или учебная учетная запись)     | Calendars.ReadWrite                         |
| Делегированные (личная учетная запись Майкрософт) | Calendars.ReadWrite                         |
| Для приложений                            | Calendars.ReadWrite                         |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

Объект [calendarGroup](../resources/calendargroup.md) по умолчанию для пользователя.

```http
POST /me/calendars
POST /users/{id | userPrincipalName}/calendars
```

Любой объект [calendarGroup](../resources/calendargroup.md) пользователя.

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок        | Значение                       |
| :------------ | :-------------------------- |
| Авторизация | Bearer {токен}. Обязательный.   |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса

Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `201 Created` и объект [calendar](../resources/calendar.md) в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADYAAAR9NR5AAA="],
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/beta/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars
Content-type: application/json

{
  "name": "Marketing calendar"
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-calendar-from-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-calendar-from-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-calendar-from-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-calendar-from-calendargroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


Предоставьте в тексте запроса описание объекта [calendar](../resources/calendar.md) в формате JSON.

##### <a name="response"></a>Отклик

Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('68ca8ec0-11f8-456b-a785-70d9936650d5')/calendarGroups('AAMkADYAAAR9NR5AAA%3D')/calendars/$entity",
    "id": "AAMkADYCQM0GfRAAAcrRD-AAA=",
    "name": "Marketing calendar",
    "color": "auto",
    "changeKey": "4xTfgHLeDkOqYVAkDNBn0QAAHKl46A==",
    "canShare": true,
    "canViewPrivateItems": true,
    "canEdit": true,
    "owner": {
        "name": "Adele Vance",
        "address": "adelev@contoso.OnMicrosoft.com"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


