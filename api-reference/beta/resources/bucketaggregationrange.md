---
title: Тип ресурса Буккетаггрегатионранже
description: 'Позволяет указать несколько ручных диапазонов в запросе статистической обработки. Это относится только к уточнениям без строки: числа и даты.'
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 77f89503a8f19bd8b057575643ebf89e6dbc43a8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193980"
---
# <a name="bucketaggregationrange-resource-type"></a>Тип ресурса Буккетаггрегатионранже

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задает нижнюю и верхнюю границу диапазона для агрегирования результатов поиска. Применяется только к уточнениям даты или числового типа.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|from|String| Определяет нижнюю границу, от которой вычисляется агрегация. Это может быть числовое значение или строковое представление даты с использованием `YYYY-MM-DDTHH:mm:ss.sssZ` формата. Обязательно.|
|на|String| Определяет верхнюю границу, до которой вычисляется агрегация. Это может быть числовое значение или строковое представление даты с использованием `YYYY-MM-DDTHH:mm:ss.sssZ` формата. Обязательный элемент.|

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
