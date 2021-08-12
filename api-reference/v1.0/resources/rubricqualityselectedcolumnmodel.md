---
title: rubricQualitySelectedColumnModel type
description: Указывает rubricLevel, выбранный преподавателем при классификации educationRubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bef762ca4928dbde1d8e15ead4520af0dd1aa36502b74a1ed6d100a2d0480c28
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246607"
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

