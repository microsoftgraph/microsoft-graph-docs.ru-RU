---
title: тип ресурса averageComparativeScore
description: Содержит различные оценки, основанные на различных областях.
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eb78b045105725d8151d229525396fd205cd427f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089853"
---
#  <a name="averagecomparativescore-resource-type"></a>тип ресурса averageComparativeScore

Пространство имен: microsoft.graph

Содержит различные оценки в зависимости от различных областей (например, среднего по вертикали отрасли, среднего по размеру места в компании и так далее) и категории управления (Identity, Data, Device, Apps, Infrastructure).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|основы|Строка|Тип области. Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
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

