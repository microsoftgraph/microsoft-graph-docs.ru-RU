---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0305f076c4952c2e5d29df85d65f5f8d6c86232f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913760"
---
# <a name="audioduckingconfiguration-resource-type"></a>Тип ресурса Аудиодуккингконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры дуккинг других источников (фасинг в других источниках и из них).

## <a name="properties"></a>Свойства

| Свойство      | Тип     | Описание                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| ловерлевел    | Int64    | Объем источников в процентах при дуккед источников.             |
| рампактиве    | Int64    | Период времени (в миллисекундах), который требуется для дуккед источников. |
| рампинактиве  | Int64    | Период времени (в миллисекундах), который требуется для дуккед источников.  |
| упперлевел    | Int64    | Объем источников в процентах, когда источники не дуккед.         |

> **Примечание:** Длительность увеличения не может превышать 5 000 миллисекунд.

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioDuckingConfiguration"
}-->
```json
{
  "lowerLevel": 20,
  "rampActive": 1000,
  "rampInactive": 1000,
  "upperLevel": 100
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioDuckingConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
