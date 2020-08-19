---
title: Тип ресурса followupFlag
description: 'Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия. '
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 263d2c5552eabfed47210dd8d53b2ce14ba1be25
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812269"
---
# <a name="followupflag-resource-type"></a>Тип ресурса followupFlag

Пространство имен: microsoft.graph


Позволяет установить флаг в элементе, чтобы пользователь выполнит дальнейшие действия.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|completedDateTime|[dateTimeTimeZone](datetimetimezone.md)|Дата и время, когда выполнение было завершено.|
|dueDateTime|**dateTimeTimeZone**|Дата и время выполнения дальнейших действий. **Примечание**. чтобы задать дату выполнения, необходимо также указать значение, в `startDateTime` противном случае будет получен `400 Bad Request` отклик.|
|flagStatus|фолловупфлагстатус|Состояние выполнения для элемента. Возможные значения: `notFlagged`, `complete` и `flagged`.|
|startDateTime|**dateTimeTimeZone**|Дата и время, когда следует начать выполнение.|

## <a name="json-representation"></a>Представление в формате JSON

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
