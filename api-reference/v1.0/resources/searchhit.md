---
title: тип ресурса searchHit
description: Описание объекта searchHit
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e64d4d3a2d7599df3ce6674abab352ab474ae18f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137548"
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

