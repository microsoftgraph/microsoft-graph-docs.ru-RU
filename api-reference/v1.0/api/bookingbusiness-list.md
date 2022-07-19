---
title: Перечисление bookingBusinesses
description: Получение коллекции объектов bookingBusiness, созданных для клиента.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: deed802ca412e3b44e4e16e2798fb82af60ae6ab
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856024"
---
# <a name="list-bookingbusinesses"></a>Перечисление bookingBusinesses

Пространство имен: microsoft.graph

Получение коллекции объектов [bookingBusiness](../resources/bookingbusiness.md) , созданных для клиента.

Эта операция возвращает только **идентификатор и** **displayName** каждого Microsoft Bookings в коллекции. Для соображений производительности он не возвращает другие свойства. Вы можете получить другие свойства компании Bookings, указав его **идентификатор** в операции [GET](bookingbusiness-get.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Приложение | BookingsAppointment.ReadWrite.All, Bookings.Read.All  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /solutions/bookingBusinesses
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает $count и $expand параметров [запроса OData](/graph/query-parameters) для настройки ответа.

Этот метод также поддерживает параметр `query` , который принимает строковое значение. Этот параметр ограничивает результаты GET организациями, которые соответствуют указанной строке. Дополнительные сведения см. в [примере](#request-2).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [bookingBusiness](../resources/bookingbusiness.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-bookings-businesses-in-a-tenant"></a>Пример 1. Получение компаний Bookings в клиенте

#### <a name="request-1"></a>Запрос 1

Следующий пример возвращает компании Bookings в клиенте.

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
```

#### <a name="response-1"></a>Отклик 1

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"Contosolunchdelivery@contoso.onmicrosoft.com",
            "displayName":"Contoso lunch delivery",
        },
        {
            "id":"Fabrikam@contoso.onmicrosoft.com",
            "displayName":"Fabrikam",
        }
    ]
}
```

### <a name="example-2-use-query-to-get-one-or-more-matching-bookings-businesses-in-a-tenant"></a>Пример 2. Использование запроса для получения одного или нескольких соответствующих компаний Bookings в клиенте

#### <a name="request-2"></a>Запрос 2

В следующем примере показано, как использовать параметр `query` для получения одного или нескольких соответствующих компаний Bookings в клиенте.

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses?query=Adventure
```

#### <a name="response-2"></a>Ответ 2

Ниже приведен пример отклика.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/v1.0/solutions/$metadata#bookingBusinesses",
    "value":[
        {
            "id":"AdventureWorksCycles@M365B960066.onmicrosoft.com",
            "displayName":"Adventure Works Cycles",
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List bookingBusinesses",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
