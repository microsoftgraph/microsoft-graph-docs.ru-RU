---
title: тип ресурса sortProperty
description: Указывает порядок сортировки результатов поиска
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 822819ba68ba6786da111d8976c76fdcd30e591d
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514354"
---
# <a name="sortproperty-resource-type"></a>тип ресурса sortProperty

Пространство имен: microsoft.graph

Указывает порядок сортировки результатов поиска.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|name|String|Имя свойства для сортировки. Обязательно.|
|isDescending|Логический|`True` если порядок сортировки будет нисходящим. По умолчанию `false` , с порядком сортировки как восходящий. Необязательное свойство.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sortProperty",
  "baseType": null
}-->

```json
{
  "name": "String",
  "isDescending": "true"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sortProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->