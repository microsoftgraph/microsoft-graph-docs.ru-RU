---
title: " Тип ресурса Аверажекомпаративескоре"
description: Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).
localization_priority: Normal
ms.openlocfilehash: c32c1349edd70e80c1bf0fb12a36bd07e06ed39f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535440"
---
#  <a name="averagecomparativescore-resource-type"></a>Тип ресурса Аверажекомпаративескоре

Этот ресурс содержит различные показатели, основанные на разных областях (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).

|Свойство |Тип |Описание |
|:--|:--|:--|
|   бы   |   String  |   Тип области (по Аллтенантс, Тоталсеатс, Индустритипес).  |
|   Аверажескоре    |   Двойное  | Средняя оценка в указанном базисе. |
|   Девицескоре |   Двойное  | Средняя оценка в указанном базисе. |
|   Score   |   Двойное  | Средняя оценка в указанном базисе. |
|   Идентитискоре   |   Двойное  | Средняя оценка в указанном базисе. |

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
