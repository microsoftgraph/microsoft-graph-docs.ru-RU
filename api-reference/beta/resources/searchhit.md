---
title: Тип ресурса Сеарчхит
description: Описание объекта Сеарчхит
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c140a30d4e77840b1fd7c7ccceec16e0554cd855
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193612"
---
# <a name="searchhit-resource-type"></a>Тип ресурса Сеарчхит

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Представляет один результат в списке результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|хитид|String|Внутренний идентификатор элемента.|
|rank|Int32|Ранг или порядок результатов.|
|contentSource|String|Имя источника контента, частью которого является **екстерналитем** .|
|summary|String|Сводка результатов, если доступна сводка.|
|resource|[entity](entity.md)|Базовое представление результатов поиска в Microsoft Graph.|
|_id (устаревшее)|String| Переименован в качестве **хитид**. Внутренний идентификатор элемента.|
|_score (устаревшее)|Int32|Переименовано в качестве **ранга**. Оценка или порядок результатов.|
|_summary (устаревшее)|String|Переименовано в качестве **сводки**. Сводка результатов (если доступна сводка).|
|_sortField (устаревшее)|String|Это свойство было удалено.|
|_source (устаревшее)|[entity](entity.md)|Переименовано в качестве **ресурса**. Базовое представление результата поиска на диаграмме.|

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
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
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

