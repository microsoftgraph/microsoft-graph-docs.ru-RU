---
title: Обновление bookingservice
description: Обновление свойства объекта bookingService в указанном bookingbusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519719"
---
# <a name="update-bookingservice"></a>Обновление bookingservice

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойства объекта [bookingService](../resources/bookingservice.md) в указанном [bookingbusiness](../resources/bookingbusiness.md).

Ниже приведены некоторые примеры, которые можно настроить для службы:
- Price
- Типичная длина встречи
- Reminders
- Любой буфер времени для настройки перед или завершить после службы
- [Планирование политики](../resources/bookingschedulingpolicy.md) параметров, таких как минимальные уведомление о книги или отменить, и ли клиенты могут выбрать элементы определенного персонала для встречи.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) |  Bookings.ReadWrite.All Bookings.Manage.All   |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.   |
|Для приложений | Не поддерживается.  |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a>Необязательные заголовки запросов
| Имя       | Описание|
|:-----------|:-----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|defaultDuration|Длительность|Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд. Например P11D23H59M59.999999999999S. |
|defaultLocation|[location](../resources/location.md)|Физическое расположение по умолчанию для службы.|
|defaultPrice|Double|Денежные Цена по умолчанию для службы.|
|defaultPriceType|string|По умолчанию способ службу оценивается. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md) коллекции|Значение по умолчанию набора оповещения о встрече этой службы. Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.|
|description|Строка|Текстовое описание для службы.|
|displayName|String|Имя службы.|
|emailAddress|String|Адрес электронной почты|
|id|String| Только для чтения.|
|isHiddenFromCustomers|Логическое|Значение true означает, что эта служба недоступна для клиентов для резервирования.|
|notes|String|Дополнительные сведения об этой службы.|
|postBuffer|Длительность|Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.|
|пребуфер|Длительность|Время для буфера до начала встречи для этой службы.|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.|
|staffMemberIds|Коллекция String|Представляет эти [Сотрудники](../resources/bookingstaffmember.md) , предоставляющих этой службы. |

## <a name="response"></a>Ответ
При успешном выполнении этот метод возвращает код отклика `204 No content`. Метод не возвращает данные в теле отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере обновляются длительность указанной службы.
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a>Ответ
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
