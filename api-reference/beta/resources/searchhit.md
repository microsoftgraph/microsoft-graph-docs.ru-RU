---
title: тип ресурса searchHit
description: Описание объекта searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c546483eea81e7d89a3a87ba5b8c0eb0ff48783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210334"
---
# <a name="searchhit-resource-type"></a>тип ресурса searchHit

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Представляет один результат в списке результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hitId|String|Внутренний идентификатор элемента.|
|rank|Int32|Ранж или порядок результата.|
|contentSource|String|Имя источника контента, **частью которого является externalItem.**|
|summary|String|Сводка результатов, если резюме доступно.|
|resultTemplateId|String|ID шаблона результатов для отрисовки результата поиска. Этот ID должен отображать макет в словаре **resultTemplates,** который также включен в [searchresponse.](searchresponse.md)|
|resource|[entity](entity.md)|В основном microsoft Graph представление результата поиска.|
|_id (неподготовленный)|String| Переименован в **hitId**. Внутренний идентификатор элемента.|
|_score (обесценилось)|Int32|Переименован в **ранж.** Оценка или порядок результата.|
|_summary (обесценилось)|String|Переименовано в **сводку**. Сводка результатов (если сводка доступна).|
|_sortField (обесценилось)|String|Это свойство удалено.|
|_source (обесценилось)|[entity](entity.md)|Переименован в **ресурс.** В Graph представлен результат поиска.|

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
  "resultTemplateId": "String",
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

