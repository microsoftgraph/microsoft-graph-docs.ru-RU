---
title: Тип ресурса Сеарчаггрегатион
description: Предоставляет сведения о агрегате поиска в ответе поиска.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 480a6f70a2815a174697ff22fc217057053e1f4b
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193964"
---
# <a name="searchaggregation-resource-type"></a>Тип ресурса Сеарчаггрегатион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет сведения о агрегате поиска в ответе поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|displayName|String| Понятное имя объединения. Это значение было указано во входных данных.|
|поле|String| Определяет, для какого поля вычислена агрегация.|
|buckets|Коллекция [сеарчбуккет](searchbucket.md)| Определяет фактические сегменты вычисленной статистической обработки.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAggregation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "field": "String",  
  "buckets": [{"@odata.type": "microsoft.graph.searchBucket"}]
}
```