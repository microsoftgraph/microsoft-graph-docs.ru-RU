---
title: Создание или замена расписания
description: Создание или замена объекта **расписания.**
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 02196fab37f28a2ab8f669ff4427d7512a0f0348
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786336"
---
# <a name="create-or-replace-schedule"></a>Создание или замена расписания

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание или замена объекта [расписания.](../resources/schedule.md)

Процесс создания расписания соответствует рекомендациям One API для длительных операций на основе ресурсов [(RELO).](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)
Если клиенты используют метод PUT, если расписание является предварительным, операция заменяет расписание; в противном случае операция запускает процесс подготовки расписания в фоновом режиме.

При расписании клиенты могут использовать метод [GET,](schedule-get.md) чтобы получить расписание и посмотреть свойство для текущего состояния `provisionStatus` подготовка. Если подготовка не удалась, клиенты могут получить дополнительные сведения из `provisionStatusCode` свойства.

Клиенты также могут проверить конфигурацию расписания.


## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Schedule.ReadWrite.All, Group.ReadWrite.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | Schedule.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a>Заголовки запросов

| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем JSON-представление объекта [расписания.](../resources/schedule.md)

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` объект [расписания](../resources/schedule.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-update-a-schedule"></a>Пример 1. Обновление расписания

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/team-put-schedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]


#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null,
  "timeClockEnabled": true,
  "openShiftsEnabled": true,
  "swapShiftsRequestsEnabled": true,
  "offerShiftRequestsEnabled": true,
  "timeOffRequestsEnabled": true
}
```

### <a name="example-2-enable-location-detection-for-time-clock"></a>Пример 2. Включить обнаружение местоположения для часов времени

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/871dbd5c-3a6a-4392-bfe1-042452793a50/schedule

{
   "enabled":true,
   "timeZone":"America/Chicago",
   "provisionStatus":"Completed",
   "provisionStatusCode":null,
   "openShiftsEnabled":true,
   "swapShiftsRequestsEnabled":true,
   "offerShiftRequestsEnabled":true,
   "timeOffRequestsEnabled":true,
   "timeClockEnabled":true,
   "timeClockSettings":{
      "approvedLocation":{
         "altitude":1024.13,
         "latitude":26.13246,
         "longitude":24.34616
      }
   }
} 
```

#### <a name="response"></a>Отклик

Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
   "enabled":true,
   "timeZone":"America/Chicago",
   "provisionStatus":"Completed",
   "provisionStatusCode":null,
   "openShiftsEnabled":true,
   "swapShiftsRequestsEnabled":true,
   "offerShiftRequestsEnabled":true,
   "timeOffRequestsEnabled":true,
   "timeClockEnabled":true,
   "timeClockSettings":{
      "approvedLocation":{
         "altitude":1024.13,
         "latitude":26.13246,
         "longitude":24.34616
      }
   }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


