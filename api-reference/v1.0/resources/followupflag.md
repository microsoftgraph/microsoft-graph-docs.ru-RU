---
title: Тип ресурса followupFlag
description: 'Позволяет установить флаг в элементе для последующего действия пользователя. '
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9b690c86a6ccbef6f5c215e268f7b34243e3023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130208"
---
# <a name="followupflag-resource-type"></a>Тип ресурса followupFlag

Пространство имен: microsoft.graph


Позволяет установить флаг в элементе для последующего действия пользователя.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата и время, когда выполнение было завершено.|
|dueDateTime|**dateTimeTimeZone**|Дата и время завершения последующего действия. **Примечание.** Чтобы задать дату окончания, необходимо также указать; в противном случае вы `startDateTime` получите `400 Bad Request` ответ.|
|flagStatus|followupFlagStatus|Состояние выполнения для элемента. Возможные значения: `notFlagged`, `complete` и `flagged`.|
|startDateTime|**dateTimeTimeZone**|Дата и время, когда следует начать выполнение.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

