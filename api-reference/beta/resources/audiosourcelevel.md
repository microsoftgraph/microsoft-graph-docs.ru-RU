---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb98e434540dd00529963c48ff3f3296e17e0c01
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998952"
---
# <a name="audiosourcelevel-resource-type"></a>Тип ресурса Аудиосаурцелевел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка уровня для других источников.

## <a name="properties"></a>Свойства

| Свойство               | Тип    | Описание                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| дуккосерс             | Boolean | Позволяет этому источнику дукк другие источники в активном состоянии. Если задано значение true, необходимо задать уровень дуккинг.|
| степень                  | Int64   | Дуккинг уровень источника, если `duckOthers` задано значение `true` .                                     |
| participant            | String  | Поток звука участника источника.                                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


