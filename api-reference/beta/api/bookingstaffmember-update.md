---
title: Обновление bookingstaffmember
description: Обновите свойства объекта bookingStaffMember в указанном bookingbusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3aa430d1e59bf3506dc7d1bbfd3dc4083e2f9fbe
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160460"
---
# <a name="update-bookingstaffmember"></a>Обновление bookingstaffmember

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновите свойства [объекта bookingStaffMember](../resources/bookingstaffmember.md) в указанном [bookingBusiness](../resources/bookingbusiness.md).
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Bookings.ReadWrite.All, Bookings.Manage.All   |
|Делегированное (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Носитель {code}. Обязательно.|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|Значение true означает, что если сотрудник является Microsoft 365 пользователем, API Bookings использует личный календарь сотрудника в Microsoft 365 а также свойство **workingHours** для определения доступности. |
|colorIndex|Int32|Определяет цвет, представляющий сотрудника. Цвет соответствует цветовой палитре на странице **сведений** о персонале в приложении Bookings.|
|displayName|Строка|Имя сотрудника, отображаемое клиентам.|
|emailAddress|String|Адрес электронной почты сотрудника. Он может быть в том же Microsoft 365, что и бизнес, или в другом домене электронной почты. Этот адрес электронной почты используется, если свойство **sendConfirmationsToOwner** имеет значение true в политике планирования бизнеса.|
|isEmailNotificationEnabled|Boolean|Значение true означает, что сотрудник будет получать уведомления по электронной почте при создании или изменении назначенного ему резервирования.
|role|string| Роль сотрудника в организации. Возможные значения: `guest`, `administrator`, `viewer`, `scheduler`, `member`, `externalGuest`.|
|timeZone|String|Часовой пояс сотрудника. Список возможных значений см. в [разделе dateTimeTimeZone](../resources/datetimetimezone.md).|
|useBusinessHours|Boolean|Значение true означает, что доступность сотрудника определяется **свойством businessHours** компании. Значение false означает, что доступность определяется параметром свойства **workingHouse** сотрудника.|
|workingHours|[Коллекция bookingWorkHours](../resources/bookingworkhours.md)|Диапазон часов каждый день недели, в течение которого сотрудник доступен для резервирования.|

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере расписание сотрудника изменяется на выходные понедельники.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingstaffmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-bookingstaffmember-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-bookingstaffmember-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Отклик
Ниже приведен пример отклика.
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
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


