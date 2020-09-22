---
title: Тип ресурса Сеарчхит
description: УКАЖИТЕ ОПИСАНИЕ
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3d010f3731fa65e1ab2dc3abbf84ffdc5ebdb732
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985778"
---
# <a name="searchhit-resource-type"></a>Тип ресурса Сеарчхит

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет один результат в списке результатов поиска.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|_id|String|Внутренний идентификатор элемента.|
|_score|Int32|Оценка или порядок результатов.|
|_sortField|String|Используемый порядок сортировки. Это может быть значение DateTime или релевантность.|
|_summary|String|Сводка результатов (если доступна сводка).|
|_source|[entity](entity.md)|Базовое представление результата поиска на диаграмме.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

