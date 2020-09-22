---
title: Тип ресурса Усажедетаилс
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) или изменился (редактируется) пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 553de0e8df9b3853024ffc35cc61bf6d727a2c9b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986077"
---
# <a name="usagedetails-resource-type"></a>Тип ресурса Усажедетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [используемых](insights-used.md) элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) или изменился (редактируется) пользователем.


## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a>Свойства

| Свойство              | Тип          | Описание  |
| -------------         |---------------| -------------|
| lastAccessedDateTime                  | DateTimeOffset        | Дата и время последнего обращения пользователя к ресурсу. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.                      |
| lastModifiedDateTime              | DateTimeOffset        | Дата и время последнего изменения ресурса пользователем. Метка времени представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `2014-01-01T00:00:00Z`. Только для чтения.       |


