---
title: Перечисление служб
description: Получение списка объектов bookingService в указанном bookingbusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: eb7291666458b827af917970c07ed063ed71b468
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755581"
---
# <a name="list-services"></a>Перечисление служб

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [bookingService](../resources/bookingservice.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированное (рабочая или учебная учетная запись) |  Bookings. Read.All, BookingsAppointment.ReadWrite.All, Bookings. ReadWrite.All, Bookings. Manage.All   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.   |
|Application | BookingsAppointment.ReadWrite.All, Bookings. Read.All  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Носитель {code}. Обязательно.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.
## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [bookingService](../resources/bookingservice.md) в тексте отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-services-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-services-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример ответа. 

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40contoso.onmicrosoft.com')/services",
    "value": [
        {
            "id": "f9b9121f-aed7-4c8c-bb3a-a1796a0b0b2d",
            "displayName": "Initial service",
            "defaultDuration": "PT10M",
            "defaultPrice": 0,
            "defaultPriceType": "notSet",
            "description": "Not sure how to choose? Let us introduce you to our traditional family recipes.",
            "isHiddenFromCustomers": false,
            "notes": "This is where you can add notes about this service that only you and your staff see.",
            "preBuffer": "PT0S",
            "postBuffer": "PT0S",
            "staffMemberIds": [],
            "isLocationOnline": true,
            "smsNotificationsEnabled": true,
            "webUrl": "https://outlook.office365.com/owa/calendar/Contosolunchdelivery@contoso.onmicrosoft.com/bookings/s/gkcGIq92Z0u5h4ABB9Qgce5",
            "schedulingPolicy": null,
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": []
        },
        {
            "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "displayName": "Catered bento",
            "defaultDuration": "PT30M",
            "defaultPrice": 10,
            "defaultPriceType": "fixedPrice",
            "description": "Catered individual bento box lunch",
            "isHiddenFromCustomers": false,
            "notes": "Home-cooked special",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "staffMemberIds": [],
            "isLocationOnline": true,
            "smsNotificationsEnabled": false,
            "webUrl": "https://outlook.office365.com/owa/calendar/Contosolunchdelivery@contoso.onmicrosoft.com/bookings/s/gpcGIq92Z0u5h6ABB9Qgrt5",
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        },
        {
            "id": "635a7b7c-4230-4d3b-a42b-698e89927528",
            "displayName": "Kaiseki",
            "defaultDuration": "PT1H30M",
            "defaultPrice": 30,
            "defaultPriceType": "fixedPrice",
            "description": "Individual kaiseki lunch delivery",
            "isHiddenFromCustomers": false,
            "notes": "Home-cooked special",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "staffMemberIds": [],
            "isLocationOnline": true,
            "smsNotificationsEnabled": true,
            "webUrl": "https://outlook.office365.com/owa/calendar/Contosolunchdelivery@contoso.onmicrosoft.com/bookings/s/bplGIq92Z0u5h4FWB9Qgvu7",
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
