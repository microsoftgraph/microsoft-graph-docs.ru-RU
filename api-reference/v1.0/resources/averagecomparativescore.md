---
title: тип ресурса averageComparativeScore
description: Содержит различные оценки, основанные на различных областях.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2041a366fcf37ff8a850fb8d6fd41e9c3fd6002a17916d41718588674a30a3e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147023"
---
#  <a name="averagecomparativescore-resource-type"></a>тип ресурса averageComparativeScore

Пространство имен: microsoft.graph

Содержит различные оценки в зависимости от различных областей (например, среднего по вертикали отрасли, среднего по размеру места в компании и так далее) и категории управления (Identity, Data, Device, Apps, Infrastructure).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|основы|String|Тип области. Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
|averageScore|Двойное с плавающей точкой|Средний балл в пределах указанной основы.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

