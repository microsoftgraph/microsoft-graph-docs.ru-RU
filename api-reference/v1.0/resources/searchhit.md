---
title: тип ресурса searchHit
description: Описание объекта searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3cc9d069e91dd8c8d51ba6b010c2c3ccc9dad01ac01695d6782e99bffea973e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138331"
---
# <a name="searchhit-resource-type"></a>тип ресурса searchHit

Пространство имен: microsoft.graph

Представляет один результат в списке результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|hitId|String|Внутренний идентификатор элемента.|
|rank|Int32|Ранж или порядок результата.|
|contentSource|String|Имя источника контента, **частью которого является externalItem.**|
|summary|String|Сводка результатов, если резюме доступно.|
|resource|[entity](entity.md)|В основном microsoft Graph представление результата поиска.|

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
  "resource": { "@odata.type": "microsoft.graph.entity" }
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

