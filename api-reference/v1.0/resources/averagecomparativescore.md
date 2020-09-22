---
title: Тип ресурса Аверажекомпаративескоре
description: Содержит различные оценки на основе разных областей.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bc104f3a9c19c38ef569d08d24da83d0e07d75f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091903"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса Аверажекомпаративескоре

Пространство имен: microsoft.graph

Содержит различные оценки на основе различных областей (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).

## <a name="properties"></a>Свойства

|Свойство |Тип |Описание |
|:--|:--|:--|
|бы|Строка|Тип области. Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.|
|аверажескоре|Двойное с плавающей точкой|Средняя оценка в указанном базисе.|

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

