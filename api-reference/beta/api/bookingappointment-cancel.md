---
title: 'bookingAppointment: Отмена'
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: ffb800b5084177b05b62e1ba14b475b8a760d766
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844480"
---
# <a name="bookingappointment-cancel"></a>bookingAppointment: Отмена

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Отменить указанного [bookingAppointment](../resources/bookingappointment.md) в указанном [bookingbusiness](../resources/bookingbusiness.md)и отправить сообщение связанных клиентов и сотрудников.

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
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Тело запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|cancellationMessage|Строка|Сообщение для подтверждения с клиентом отменена встречи.|

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.

При попытке отменить встречи, которая не существует, этот метод возвращает `HTTP 404 Not found`.

## <a name="example"></a>Пример
Ниже приведен пример вызова этого API.
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "bookingappointment_cancel"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKoAAA=/cancel
Content-type: application/json

{
  "cancellationMessage": "Your appointment has been successfully cancelled. Please call us again."
}
```

##### <a name="response"></a>Ответ
Ниже приведен пример ответа. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingAppointment: cancel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
