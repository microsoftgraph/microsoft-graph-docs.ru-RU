---
title: 'bookingsBusiness: getStaffAvailability'
description: Узнайте, как получить сведения о доступности сотрудников Microsoft Bookings календаря.
ms.localizationpriority: medium
author: kwekua
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 71954be1123f5b36532380b61159934228edfc9e
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2022
ms.locfileid: "64755757"
---
# <a name="bookingsbusiness-getstaffavailability"></a>bookingsBusiness: getStaffAvailability

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение сведений о доступности [сотрудников](../resources/bookingstaffmember.md) Microsoft Bookings [календаря](../resources/bookingappointment.md).

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Не поддерживается.   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Application | Calendar.Read, Calendar.ReadWrite, Bookings. Read.All, Calendars.ReadWrite  |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->
```http
Get /solutions/bookingBusinesses/{id}/getStaffAvailability

```

## <a name="request-header"></a>Заголовок запроса

|Имя |Описание |
|:--------------|:------------|
|Авторизация |Носитель {code}. Обязательно. |
|Content-Type| application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса передайте список идентификаторов сотрудников вместе с двумя другими параметрами типа ресурса [dateTimeTimeZone](/graph/resources/datetimetimezone) , которые **называются startDateTime** и **endDateTime**. Они соответствуют двум меткам времени, между которыми будет возвращена доступность персонала.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию [staffAvailabilityItem](../resources/staffavailabilityitem.md) в ответе.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getstaffavailability"
}-->

```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/getStaffAvailability 
Content-Type: application/json 

{ 
    "staffIds": [ 
        "311a5454-08b2-4560-ba1c-f715e938cb79" 
    ], 
    "startDateTime": { 
        "dateTime": "2022-01-25T00: 00: 00", 
        "timeZone": "India Standard Time" 
    }, 
    "endDateTime": { 
        "dateTime": "2022-01-26T17: 00: 00", 
        "timeZone": "Pacific Standard Time" 
    } 
}
```

### <a name="response"></a>Отклик

Ниже приводится пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.staffAvailabilityItem",
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{ 
    "staffAvailabilityItem": [ 
        { 
            "staffId": "311a5454-08b2-4560-ba1c-f715e938cb79", 
            "availabilityItems": [ 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T15:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Busy", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T15:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T16:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-24T16:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-24T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-25T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-25T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                }, 
                { 
                    "status": "Available", 
                    "startDateTime": { 
                        "dateTime": "2022-01-26T08:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "endDateTime": { 
                        "dateTime": "2022-01-26T17:00:00", 
                        "timeZone": "(UTC-08:00) Pacific Time (US & Canada)" 
                    }, 
                    "serviceId": "" 
                } 
            ] 
        } 
    ] 
}
```
<!-- 
In the response body, for each staff member, their available windows are returned. The types of status of the windows are explained below.

|Type      | Explanation              |
|:--------------------|:---------------------------------------------------------|
|Available | The staff member is available in the given window.   |
|slotAvailable | The staff member has an appointment in the given window. The appointment is for a service which has **maxAttendeecount** more than 1. The customer can join this appointment as there are empty slots available.   |
|Busy | The staff member has an appointment in the given window. Either the staff member has an appointment for a service which has **maxAttendeecount** equal to 1 or the staff has an appointment for a service with **maxAttendeecount** more than 1 but without any available slots.  |


-->
