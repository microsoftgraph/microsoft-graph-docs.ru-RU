---
title: Тип ресурса Усажедетаилс
description: Сложный тип, содержащий свойства используемых элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) и изменен (изменен) пользователем.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 550a71fa087870f708df2587454d9ebc05bbec1d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495524"
---
# <a name="usagedetails-resource-type"></a>Тип ресурса Усажедетаилс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сложный тип, содержащий свойства [используемых](insights-used.md) элементов. Сведения о том, когда ресурс был последний раз обращался (просматривался) и изменен (изменен) пользователем.

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
