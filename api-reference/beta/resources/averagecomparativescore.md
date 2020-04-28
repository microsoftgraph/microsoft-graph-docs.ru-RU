---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e051ee3d1265c1dc65a5ab0cb9352d9cd536b21c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508054"
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
