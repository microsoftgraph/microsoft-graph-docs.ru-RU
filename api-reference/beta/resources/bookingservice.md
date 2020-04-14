---
title: Тип ресурса Букингсервице
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 53c5bc6be0953c68dc431be04b17f582715582c0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43448369"
---
# <a name="bookingservice-resource-type"></a>Тип ресурса Букингсервице

Пространство имен: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Представляет сведения о конкретной службе, предоставляемой [букингбусинесс](bookingbusiness.md), такие как имя службы, Цена и сотрудники, которые обычно предоставляют такую службу.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список служб](../api/bookingbusiness-list-services.md) | Коллекция [букингсервице](bookingservice.md) | Получение списка объектов **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).|
|[Создание Букингсервице](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Создайте объект **букингсервице** для указанного [букингбусинесс](../resources/bookingbusiness.md). |
|[Получение Букингсервице](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Получение свойств и связей объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md).|
|[обновление](../api/bookingservice-update.md). | [bookingService](bookingservice.md)    |Обновление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md). |
|[удаление](../api/bookingservice-delete.md); | Нет |Удаление объекта **букингсервице** в указанном [букингбусинесс](../resources/bookingbusiness.md). |

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|дефаултдуратион|Длительность|Длина службы по умолчанию, представленная в виде числа дней, часов, минут и секунд. Например, P11D23H59M 59.999999999999 S. |
|defaultLocation|[location](location.md)|Физическое расположение службы по умолчанию.|
|дефаултприце|Двойное с плавающей точкой|Денежная Цена по умолчанию для службы.|
|дефаултприцетипе|string|Способ оплаты службы по умолчанию. Возможные значения: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|дефаултреминдерс|Коллекция [букингреминдер](bookingreminder.md)|Набор напоминаний по умолчанию для встречи этой службы. Значение этого свойства доступно только при чтении этого **букингсервице** с помощью идентификатора.|
|description|String|Текстовое описание службы.|
|displayName|Строка|Имя службы.|
|emailAddress|String|Адрес электронной почты|
|id|Строка|Идентификатор этой службы в формате GUID. Только для чтения.|
|ишидденфромкустомерс|Логическое|Значение true означает, что эта служба недоступна клиентам для резервирования.|
|notes|String|Дополнительные сведения об этой службе.|
|Буфер буфера|Длительность|Время, в течение которого помещается в буфер после встречи для этой службы и до того, как может быть зарезервирована Следующая встреча покупателя.|
|пребуфер|Длительность|Время, в течение которого будет помещено в буфер, прежде чем можно будет запустить встречу для этой службы.|
|счедулингполици|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|Набор политик, определяющих, как должны создаваться встречи для этого типа службы и управлять ими.|
|стаффмемберидс|Коллекция String|Представляет [сотрудников](bookingstaffmember.md) , которые предоставляют эту службу. |

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
