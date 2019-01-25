---
title: Тип ресурса bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 35e439888b39c81451242f01d2aaae89b65ad8ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519887"
---
# <a name="bookingservice-resource-type"></a>Тип ресурса bookingService

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сведения об определенной службы, предоставляемые [bookingBusiness](bookingbusiness.md), такие как имя службы, цены и персонала, который обычно предоставляет такие службы.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список служб](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md) коллекции | Получите список объектов **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Создание bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Создание **bookingService** для указанного [bookingbusiness](../resources/bookingbusiness.md). |
|[Получение bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Получите свойства и связи объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Update](../api/bookingservice-update.md) | [bookingService](bookingservice.md)    |Обновление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Delete](../api/bookingservice-delete.md) | Нет |Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|defaultDuration|Длительность|Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд. Например P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|Физическое расположение по умолчанию для службы.|
|defaultPrice|Double|Денежные Цена по умолчанию для службы.|
|defaultPriceType|string|По умолчанию способ службу оценивается. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](bookingreminder.md) коллекции|Значение по умолчанию набора оповещения о встрече этой службы. Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.|
|description|Строка|Текстовое описание для службы.|
|displayName|String|Имя службы.|
|emailAddress|String|Адрес электронной почты|
|id|String|Идентификатор службы, в формате GUID. Только для чтения.|
|isHiddenFromCustomers|Логическое|Значение true означает, что эта служба недоступна для клиентов для резервирования.|
|notes|String|Дополнительные сведения об этой службы.|
|postBuffer|Длительность|Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.|
|пребуфер|Длительность|Время для буфера до начала встречи для этой службы.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.|
|staffMemberIds|Коллекция String|Представляет эти [Сотрудники](bookingstaffmember.md) , предоставляющих этой службы. |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": "string",
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "staffMemberIds": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingservice.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
