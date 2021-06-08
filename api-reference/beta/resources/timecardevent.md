---
title: тип ресурса timeCardEvent
description: Представляет определенное событие с хет-листом.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8be7d000b3d55368f7378e9b993b5015b7ef632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786399"
---
# <a name="timecardevent-resource-type"></a>тип ресурса timeCardEvent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет определенное [событие timeCard.](timecard.md)

## <a name="properties"></a>Свойства
|Свойство               |Тип           |Описание                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| dateTime                  |`Edm.dateTimeOffset`  |Время записи. |
| atApprovedLocation |`Edm.boolean `  |Указывает, была ли запись записана в утвержденное расположение. |
| notes                 |[itemBody](itembody.md)  | Заметки о **timeCardEvent**.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEvent"
}-->
```json
{
   "atApprovedLocation":true,
   "notes":{ "@odata.type":"microsoft.graph.itemBody" }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
