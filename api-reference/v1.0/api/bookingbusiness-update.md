---
title: Обновление bookingbusiness
description: Обновление свойств объекта bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3e86b5815999dc4c7388f00dd8077bed0fb1b906
ms.sourcegitcommit: 086e9a2ccaef411f9471cca164a79197bb254521
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2022
ms.locfileid: "62014168"
---
# <a name="update-bookingbusiness"></a>Обновление bookingbusiness

Пространство имен: microsoft.graph

Обновление свойств объекта [bookingBusiness.](../resources/bookingbusiness.md)
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /solutions/bookingBusinesses/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|address|[physicalAddress](../resources/physicaladdress.md)|Адрес улицы бизнеса. Тип **атрибута** physicalAddress не поддерживается в v1.0. Внутренне мы относям адреса к типу `others` .|
|businessHours|[коллекция bookingWorkHours](../resources/bookingworkhours.md)|Часы работы для бизнеса.|
|businessType|Строка|Тип бизнеса.|
|defaultCurrencyIso|Строка|Код валюты, в которую бизнес работает в Microsoft Bookings.|
|displayName|String|Имя для бизнеса, который взаимодействует с клиентами.|
|email|String|Адрес электронной почты для бизнеса.|
|phone|String|Номер телефона для бизнеса.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Указывает, как можно создавать заказы для этого бизнеса.|
|webSiteUrl|Строка|URL-адрес веб-сайта бизнеса.|

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере обновляется бизнес-адрес электронной почты и политика планирования, чтобы изменить интервал времени бронирования по умолчанию для бизнеса на час, а также предварительное бронирование до 30 дней.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/fabrikam@contoso.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```

### <a name="response"></a>Отклик
Ниже представлен пример ответа. Примечание: показанный здесь объект ответа может быть сокращен для удобочитаемости.
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


