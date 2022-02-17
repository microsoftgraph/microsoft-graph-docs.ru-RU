---
title: тип ресурса resultTemplateOption
description: Предоставляет параметры шаблона результатов поиска для отображения результатов поиска из соединители.
ms.localizationpriority: medium
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5f1e6b30a1730bfb0e4a667b51c93a47cc3dcb12
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878707"
---
# <a name="resulttemplateoption-resource-type"></a>тип ресурса resultTemplateOption

Пространство имен: microsoft.graph

Предоставляет параметры шаблона результатов поиска для отображения результатов поиска из соединители.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|enableResultTemplate|Логический|Указывает, включены ли макеты отображения поиска. Если включено, пользователь получит шаблон результатов для отображения контента результатов поиска в **свойстве resultTemplates** [ответа](/graph/api/resources/searchresponse). Шаблон результатов основан на [адаптивных картах](https://adaptivecards.io/). Необязательное свойство. |


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resultTemplateOption",
  "baseType": null
}-->

```json
 {
    "enableResultTemplate": "Boolean"
 }
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resultTemplateOption resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
