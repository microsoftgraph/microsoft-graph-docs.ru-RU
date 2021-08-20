---
title: " тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные оценки, основанные на различных областях (например, среднее по вертикали отрасли, среднее по размеру места в компании и так далее) и категории управления (Identity, Data, Device, Apps, Infrastructure).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 7a09d3b2c6457063457eee4a4bfbe3d1f88823f8864f66ac4a1ea690e33c77e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54210150"
---
#  <a name="averagecomparativescore-resource-type"></a>тип ресурса averageComparativeScore

Пространство имен: microsoft.graph

Этот ресурс содержит различные оценки, основанные на различных областях (например, среднее по вертикали отрасли, среднее по размеру места в компании и так далее) и категории управления (Identity, Data, Device, Apps, Infrastructure).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   основы   |   Строка  |   Тип области (AllTenants, TotalSeats, IndustryTypes).  |
|   averageScore    |   Двойное с плавающей точкой  | Средний балл в пределах указанной основы. |
|   deviceScore |   Двойное с плавающей точкой  | Средний балл в пределах указанной основы. |
|   dataScore   |   Двойное с плавающей точкой  | Средний балл в пределах указанной основы. |
|   identityScore   |   Двойное с плавающей точкой  | Средний балл в пределах указанной основы. |

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
  "averageScore": "Double",
  "deviceScore": "Double",
  "dataScore": "Double",
  "identityScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


