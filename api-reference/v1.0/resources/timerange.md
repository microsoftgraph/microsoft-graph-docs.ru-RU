---
title: тип ресурса timeRange
description: Ресурс диапазона времени со временем начала и окончания.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: efd466503a2f3a8e840170c551b258310e018a0ac62f6073f4fcb1c24c2f5d85
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189214"
---
# <a name="timerange-resource-type"></a>тип ресурса timeRange

Пространство имен: microsoft.graph

Ресурс диапазона времени со временем начала и окончания.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|endTime|TimeOfDay|Время окончания для диапазона времени.|
|startTime|TimeOfDay|Время начала для диапазона времени.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeRange",
  "baseType": null
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
