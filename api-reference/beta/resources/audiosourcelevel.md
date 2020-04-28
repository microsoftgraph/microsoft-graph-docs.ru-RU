---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: beb67d906c5f159f94ab8f64863eb383286489b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508103"
---
# <a name="audiosourcelevel-resource-type"></a>Тип ресурса Аудиосаурцелевел

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Настройка уровня для других источников.

## <a name="properties"></a>Свойства

| Свойство               | Тип    | Описание                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| дуккосерс             | Boolean | Позволяет этому источнику дукк другие источники в активном состоянии. Если задано значение true, необходимо задать уровень дуккинг.|
| степень                  | Int64   | Дуккинг уровень источника, если `duckOthers` задано значение. `true`                                     |
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
