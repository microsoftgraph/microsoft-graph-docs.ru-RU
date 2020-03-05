---
title: Тип ресурса Аудиодуккингконфигуратион
description: Параметры дуккинг других источников (фасинг в других источниках и из них).
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99aa202e0048b328d97453f57d249df749f7bce5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508117"
---
# <a name="audioduckingconfiguration-resource-type"></a>Тип ресурса Аудиодуккингконфигуратион

Пространство имен: Microsoft. Graph

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
