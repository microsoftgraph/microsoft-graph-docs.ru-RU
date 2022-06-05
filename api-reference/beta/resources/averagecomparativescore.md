---
title: " Тип ресурса averageComparativeScore"
description: Этот ресурс содержит различные оценки, основанные на различных областях (например, среднее по вертикали отрасли, среднее по размеру рабочих мест компании и т. д.) и категории элементов управления (удостоверение, данные, устройство, приложения, инфраструктура).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: b5cf6482b76180a64e2ec468648a48113377114d
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900214"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса averageComparativeScore

Пространство имен: microsoft.graph

Этот ресурс содержит различные оценки, основанные на различных областях (например, среднее по вертикали отрасли, среднее по размеру рабочих мест компании и т. д.) и категории элементов управления (удостоверение, данные, устройство, приложения, инфраструктура).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   Основе   |   Строка  |   Тип области (By AllTenants, TotalSeats, IndustryTypes).  |
|   averageScore    |   Двойное с плавающей точкой  | Средняя оценка в пределах указанной основы. |
|   deviceScore |   Двойное с плавающей точкой  | Средняя оценка в пределах указанной основы. |
|   dataScore   |   Двойное с плавающей точкой  | Средняя оценка в пределах указанной основы. |
|   identityScore   |   Двойное с плавающей точкой  | Средняя оценка в пределах указанной основы. |

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


