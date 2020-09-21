---
title: Тип ресурса Тонеинфо
description: Одно событие DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5555ae61920751d63a70fdb86199ffa572dcb9be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083953"
---
# <a name="toneinfo-resource-type"></a>Тип ресурса Тонеинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Одно событие DTMF.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| секуенцеид | Int64 | Добавочный идентификатор, используемый для упорядочивания событий DTMF. |
| Новая | Строка | Возможные значения: `tone0` , `tone1` ,,,,, `tone2` `tone3` `tone4` `tone5` `tone6` ,,, `tone7` `tone8` `tone9` ,,, `star` `pound` `a` , `b` , `c` , `d` , `flash` . |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


