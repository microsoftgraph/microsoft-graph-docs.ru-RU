---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c19a8d364c681fd199bf998a6951123a1cb5da86
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339077"
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
