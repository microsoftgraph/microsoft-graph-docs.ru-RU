---
title: Тип ресурса Едукатионкаурсе
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80128524160a5f01806d36f52531383d5ab469a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095516"
---
# <a name="educationcourse-resource-type"></a>Тип ресурса Едукатионкаурсе

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о курсе для класса. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                               |
| :----------- | :----- | :---------------------------------------- |
| каурсенумбер | Строка | Уникальный идентификатор курса.         |
| description  | Строка | Описание курса.                |
| displayName  | Строка | Название курса.                       |
| externalId   | String | ИДЕНТИФИКАТОР курса из системы синхронизации. |
| subject      | String | Тема курса.                    |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


