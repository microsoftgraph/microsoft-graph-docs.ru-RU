---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 69a9e63960499fb50b34cd38986b1312a4313090
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076486"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса Аверажекомпаративескоре

Пространство имен: microsoft.graph

Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   бы   |   String  |   Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).  |
|   аверажескоре    |   Двойное с плавающей точкой  | Средняя оценка в указанном базисе. |
|   девицескоре |   Двойное с плавающей точкой  | Средняя оценка в указанном базисе. |
|   Score   |   Двойное с плавающей точкой  | Средняя оценка в указанном базисе. |
|   идентитискоре   |   Двойное с плавающей точкой  | Средняя оценка в указанном базисе. |

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


