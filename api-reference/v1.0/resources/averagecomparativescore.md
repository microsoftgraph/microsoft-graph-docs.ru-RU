---
title: Тип ресурса Аверажекомпаративескоре
description: Содержит различные оценки на основе разных областей.
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 59faa1c3dcf3f7f2b70807a74878dab796ae4d54
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629329"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса Аверажекомпаративескоре

Содержит различные оценки на основе различных областей (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|бы|String|Тип области. Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
|Аверажескоре|Двойное|Средняя оценка в указанном базисе.|

## <a name="json-representation"></a>Представление в формате JSON

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
