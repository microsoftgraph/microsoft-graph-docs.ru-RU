---
title: тип ресурса educationCourse
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 347eb92cd0b36789cc7ecce1dea72af6985ea330
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232249"
---
# <a name="educationcourse-resource-type"></a>тип ресурса educationCourse

Пространство имен: microsoft.graph

Представляет сведения о курсе для класса. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | Строка | Уникальный идентификатор для курса.         |
| description  | Строка | Описание курса.                |
| displayName  | Строка | Имя курса.                       |
| externalId   | String | ID курса из системы синхронизации. |
| subject      | String | Тема курса.                    |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCourse"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationCourse",
  "subject": "String",
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String"
}
```
