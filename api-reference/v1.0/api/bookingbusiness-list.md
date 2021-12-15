---
title: Список bookingBusinesses
description: Получите коллекцию объектов bookingbusiness, созданных для клиента.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 585de83b3e5a6ba981d4f65013e0e25149149b5e
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526912"
---
# <a name="list-bookingbusinesses"></a>Список bookingBusinesses

Пространство имен: microsoft.graph

Получите коллекцию [объектов bookingBusiness,](../resources/bookingbusiness.md) созданных для клиента.

Эта операция возвращает только **id** и **displayName** каждого бизнеса Microsoft Bookings в коллекции. Для соображений производительности он не возвращает другие свойства. Вы можете получить другие свойства бизнеса Microsoft Bookings, указав его **id** в [операции GET.](bookingbusiness-get.md)


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры $count и $expand [OData](/graph/query-parameters) для настройки ответа.

Этот метод также поддерживает `query` параметр, который принимает значение строки. Этот параметр ограничивает результаты GET предприятиями, которые соответствуют указанной строке. Дополнительные сведения см. в [примере](#request-2).

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов bookingBusiness](../resources/bookingbusiness.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="example-1-get-bookings-businesses-in-a-tenant"></a>Пример 1. Получить заказы предприятий в клиенте
#### <a name="request-1"></a>Запрос 1
В следующем примере получается бизнес Bookings в клиенте.

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses
```

#### <a name="response-1"></a>Отклик 1
Ниже приведен пример ответа.
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

### <a name="example-2-use-query-to-get-one-or-more-matching-bookings-businesses-in-a-tenant"></a>Пример 2. Использование "запроса", чтобы получить одно или несколько совпадающих предприятий Bookings в клиенте
#### <a name="request-2"></a>Запрос 2
В следующем примере показано, как использовать параметр для получения одного или более совпадающих предприятий `query` Bookings в клиенте.

<!-- {
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/solutions/bookingBusinesses?query=Adventure
```

#### <a name="response-2"></a>Ответ 2
Ниже приведен пример ответа.
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
