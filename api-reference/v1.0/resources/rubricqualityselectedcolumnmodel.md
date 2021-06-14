---
title: rubricQualitySelectedColumnModel type
description: Указывает rubricLevel, выбранный преподавателем при классификации educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9e69fa26d97684db4964ffba3d268ee1d1c11b44
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911516"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a>rubricQualitySelectedColumnModel type

Пространство имен: microsoft.graph

Указывает [rubricLevel,](rubriclevel.md) выбранный преподавателем при классификации [educationRubric](educationrubric.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|columnId|String|ID выбранного уровня для этого качества.|
|qualityId|String|ID связанного качества.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

