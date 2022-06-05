---
title: Тип ресурса averageComparativeScore
description: Содержит различные оценки, основанные на разных областях.
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 88444bfab00622a6ac8cc89a3af287650ad1af7e
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899976"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса averageComparativeScore

Пространство имен: microsoft.graph

Содержит различные оценки на основе различных областей (например, среднее по вертикали отрасли, среднее по размеру рабочих мест компании и т. д.) и категории элементов управления (удостоверение, данные, устройство, приложения, инфраструктура).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|Основе|Строка|Тип области. Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
|averageScore|Двойное с плавающей точкой|Средняя оценка в пределах указанной основы.|

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

