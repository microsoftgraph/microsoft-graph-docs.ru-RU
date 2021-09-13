---
title: тип ресурса toneInfo
description: Одно событие DTMF.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4d41f9e92864c5b56a3ef41a5907b7346af7d8ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098428"
---
# <a name="toneinfo-resource-type"></a>тип ресурса toneInfo

Пространство имен: microsoft.graph

Одно событие DTMF.

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание|
|:---------------|:--------|:----------|
| sequenceId | Int64 | Дополнительный идентификатор, используемый для заказа событий DTMF. |
| тон | тон | Возможные значения: `tone0` `tone1` , , , , , `tone2` , , `tone3` , `tone4` `tone5` `tone6` `tone7` `tone8` `tone9` `star` `pound` `a` `b` `c` `d` `flash` . |

## <a name="json-representation"></a>Представление JSON

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

