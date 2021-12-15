---
title: Обновление bookingService
description: Обновление свойств объекта bookingService в указанном bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b9e13d475bdb72a282e8acbf4dd561d03258fdca
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525211"
---
# <a name="update-bookingservice"></a>Обновление службы бронирования

Пространство имен: microsoft.graph

Обновление свойств объекта [bookingService](../resources/bookingservice.md) в указанном [bookingBusiness.](../resources/bookingbusiness.md)

Ниже приводится несколько примеров, которые можно настроить для службы:
- ЦЕНА
- Типичная продолжительность встречи
- Reminders
- Любой буфер времени, который необходимо настроить до или завершить после службы
- [Планирование параметров](../resources/bookingschedulingpolicy.md) политики, например минимальное уведомление о записи или отмене, а также возможность выбора клиентами определенных сотрудников для встречи.

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
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Авторизация  | Bearer {код}. Обязательно.|

## <a name="request-body"></a>Текст запроса
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|customQuestions|[коллекция bookingQuestionAssignment](../resources/bookingquestionassignment.md)|Это содержит набор пользовательских вопросов, связанных с определенной службой. Необязательное свойство.|
|defaultDuration|Длительность|Длина службы по умолчанию, представленная в числах дней, часов, минут и секунд. Например, P11D23H59M59.999999999999S. |
|defaultLocation|[location](../resources/location.md)|Физическое расположение службы по умолчанию.|
|defaultPrice|Double|Денежная цена по умолчанию для службы.|
|defaultPriceType|bookingPriceType|Способ заряжания службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|defaultReminders|[коллекция bookingReminder](../resources/bookingreminder.md)|Набор напоминаний по умолчанию для назначения этой службы. Значение этого свойства доступно только при чтении этого **bookingService** по его ID.|
|description|Строка|Текстовое описание службы.|
|displayName|Строка|Имя службы.|
|id|Строка| Уникальный идентификатор для **bookingService.** Только для чтения.|
|isHiddenFromCustomers|Boolean|Если `true` служба недоступна клиентам для бронирования.|
|isLocationOnline|Boolean|Если это указывает на то, что встречи `true` для службы будут проводиться в Интернете. Значение по умолчанию — `false`.|
|maximumAttendeesCount|Int32|Максимальное число клиентов, разрешенных в службе.  |
|notes|String|Дополнительные сведения об этой службе.|
|postBuffer|Длительность|Время буферизации после назначения для этой службы заканчивается, и до следующей встречи клиента можно заказать.|
|preBuffer|Длительность|Время буферизации перед назначением для этой службы может начаться.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Набор политик, которые определяют, как следует создавать и управлять встречами для этого типа службы.|
|smsNotificationsEnabled|Boolean|True указывает, что sms-уведомления можно отправить клиентам для назначения службы. Значение по умолчанию − ложь.|
|staffMemberIds|Коллекция строк|Представляет тех [сотрудников,](../resources/bookingstaffmember.md) которые предоставляют эту службу. |

## <a name="response"></a>Отклик
При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
### <a name="request"></a>Запрос
В следующем примере обновляется продолжительность указанной службы.

<!-- {
  "blockType": "request"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/solutions/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа.
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


