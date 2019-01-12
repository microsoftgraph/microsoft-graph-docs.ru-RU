---
title: Тип ресурса bookingService
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 790adf49cfda1f787665a48e1b06bd77da27e1f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925163"
---
# <a name="bookingservice-resource-type"></a>Тип ресурса bookingService

 > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.
 
Представляет сведения об определенной службы, предоставляемые [bookingBusiness](bookingbusiness.md), такие как имя службы, цены и персонала, который обычно предоставляет такие службы.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список служб](../api/bookingbusiness-list-services.md) | [bookingService](bookingservice.md) коллекции | Получите список объектов **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[Создание bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Создание **bookingService** для указанного [bookingbusiness](../resources/bookingbusiness.md). |
|[Получение bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Получите свойства и связи объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md).|
|[обновление](../api/bookingservice-update.md). | [bookingService](bookingservice.md)    |Обновление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |
|[Delete](../api/bookingservice-delete.md) | Нет |Удаление объекта **bookingService** в указанном [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|defaultDuration|Продолжительность|Длина по умолчанию службы, представленный в числа дней, часов, минут и секунд. Например P11D23H59M59.999999999999S. |
|defaultLocation|[location](location.md)|Физическое расположение по умолчанию для службы.|
|defaultPrice|Double|Денежные Цена по умолчанию для службы.|
|defaultPriceType|string|По умолчанию способ службу оценивается. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](bookingreminder.md) коллекции|Значение по умолчанию набора оповещения о встрече этой службы. Значение этого свойства доступна только при чтении этой **bookingService** по идентификатору.|
|описание|Строка|Текстовое описание для службы.|
|displayName|Строка|Имя службы.|
|emailAddress|String|Адрес электронной почты|
|id|Строка|Идентификатор службы, в формате GUID. Только для чтения.|
|isHiddenFromCustomers|Логический|Значение true означает, что эта служба недоступна для клиентов для резервирования.|
|notes|String|Дополнительные сведения об этой службы.|
|postBuffer|Продолжительность|Заканчивается время буфер после встречи для этой службы и перед следующим встречи клиента можно заранее.|
|пребуфер|Продолжительность|Время для буфера до начала встречи для этой службы.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Набор политик, определяющие порядок встреч для этого типа службы следует создания и управления.|
|staffMemberIds|Коллекция String|Представляет эти [Сотрудники](bookingstaffmember.md) , предоставляющих этой службы. |

## <a name="relationships"></a>Связи
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
