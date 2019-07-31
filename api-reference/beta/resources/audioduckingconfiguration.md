---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: cfff0ca240a13c9c4396d605def05a52e1916778
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013222"
---
# <a name="audioduckingconfiguration-resource-type"></a>Тип ресурса Аудиодуккингконфигуратион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Параметры дуккинг других источников (фасинг в других источниках и из них).

## <a name="properties"></a>Свойства

| Свойство      | Тип     | Описание                                                                     |
| :------------ | :------- | :-------------------------------------------------------------------------------|
| Ловерлевел    | Int64    | Объем источников в процентах при дуккед источников.             |
| Рампактиве    | Int64    | Период времени (в миллисекундах), который требуется для дуккед источников. |
| Рампинактиве  | Int64    | Период времени (в миллисекундах), который требуется для дуккед источников.  |
| Упперлевел    | Int64    | Объем источников в процентах, когда источники не дуккед.         |

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
