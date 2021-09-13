---
title: " тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные оценки, основанные на различных областях (например, среднее по вертикали отрасли, среднее по размеру места в компании и так далее) и категории управления (Identity, Data, Device, Apps, Infrastructure).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 4c563d8754ba5afb1c4fe89d237f978d886f9eab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064611"
---
#  <a name="averagecomparativescore-resource-type"></a>тип ресурса averageComparativeScore

Пространство имен: microsoft.graph

Этот ресурс содержит различные оценки, основанные на различных областях (например, среднее по вертикали отрасли, среднее по размеру места в компании и так далее) и категории управления (Identity, Data, Device, Apps, Infrastructure).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   основы   |   String  |   Тип области (AllTenants, TotalSeats, IndustryTypes).  |
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


