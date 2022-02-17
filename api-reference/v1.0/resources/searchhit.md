---
title: тип ресурса searchHit
description: Описание объекта searchHit
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 487fbee4e501b6d4154b1ed08102730fd278730c
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878829"
---
# <a name="searchhit-resource-type"></a>тип ресурса searchHit

Пространство имен: microsoft.graph

Представляет один результат в списке результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|contentSource|String|Имя источника контента, **частью которого является externalItem** .|
|hitId|String|Внутренний идентификатор элемента.|
|rank|Int32|Ранж или порядок результата.|
|resultTemplateId|Строка|ID шаблона результатов, используемого для отображения результата поиска. Этот ID должен отображать макет в **словаре resultTemplates** , который также включен в [searchResponse](searchresponse.md).|
|resource|[entity](entity.md)|В основном microsoft Graph представление результата поиска.|
|summary|String|Сводка результатов, если резюме доступно.|

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
  "contentSource": "String",
  "hitId": "String",
  "rank": "Int32",
  "resultTemplateId": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "summary": "String"
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

