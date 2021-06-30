---
title: тип ресурса resultTemplateOption
description: Предоставляет параметры макетов отображения поиска для результатов поиска соединители визуализации.
localization_priority: Normal
author: cristianv-ms
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 404051f4eeee68ca3d5f5eb3ac6b84a23a331515
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211373"
---
# <a name="resulttemplateoption-resource-type"></a>тип ресурса resultTemplateOption

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет параметры шаблонов результатов поиска для результатов поиска соединители отрисовки.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|enableResultTemplate|Логический|Указывает, включены ли макеты отображения поиска. Если включено, пользователь получит шаблон результатов для отображения контента результатов поиска в **свойстве resultTemplates** [ответа.](/graph/api/resources/searchresponse?view=graph-rest-beta&preserve-view=true) Шаблон результатов основан на [адаптивных картах.](https://adaptivecards.io/) Это необязательное свойство.|


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
    "enableResultTemplate": true
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
