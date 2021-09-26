---
title: тип ресурса bucketAggregationRange
description: Указывает нижний и верхний предел диапазона для агрегации результатов поиска. Применяется только к переработчикам датного или числимого типа
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a101262dddd859e3c28ef0a32e117dee7546903
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767491"
---
# <a name="bucketaggregationrange-resource-type"></a>тип ресурса bucketAggregationRange

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает нижний и верхний предел диапазона для агрегации результатов поиска. Применяется только к уточнениям даты или числового типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|from|String| Определяет нижнюю границу, из которой вычисляется агрегация. Это может быть числовая величина или строка представления даты с помощью `YYYY-MM-DDTHH:mm:ss.sssZ` формата. Обязательно.|
|на|Строка| Определяет верхнюю границу, к которой необходимо вычислить агрегацию. Это может быть числовая величина или строка представления даты с помощью `YYYY-MM-DDTHH:mm:ss.sssZ` формата. Обязательный элемент.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationRange",
  "baseType": null
}-->

```json
{
  "from": "String",
  "to": "String"
}
```
