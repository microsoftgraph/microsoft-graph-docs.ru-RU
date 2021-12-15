---
title: 'bookingAppointment: отмена'
description: Отмените указанное бронированиеAppointment в указанном bookingBusiness и отправьте сообщение участвующим клиентам и сотрудникам.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 489aabcd3753e6e8796fa6a074fb6508a27ba243
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526680"
---
# <a name="bookingappointment-cancel"></a>bookingAppointment: отмена

Пространство имен: microsoft.graph

Отмените указанное [бронированиеAppointment в](../resources/bookingappointment.md) указанном [bookingBusiness](../resources/bookingbusiness.md) и отправьте сообщение участвующим клиентам и сотрудникам.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments/{id}/cancel

```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
В теле запроса укажи объект JSON со следующим параметром.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|cancellationMessage|Строка|Сообщение об отмене встречи  с клиентом.|

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.

Если вы попытаетесь отменить неуществимую встречу, этот метод возвращает  `404 Not found` .

## <a name="example"></a>Пример
Ниже приводится пример вызова этого API.
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа.
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


