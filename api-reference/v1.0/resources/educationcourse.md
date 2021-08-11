---
title: тип ресурса educationCourse
description: Представляет сведения о курсе для класса.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e54870ad3633f0b0170a54fad32ce8aa0baa2843466dd0f0e051caeacca54ffa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54135255"
---
# <a name="educationcourse-resource-type"></a>тип ресурса educationCourse

Пространство имен: microsoft.graph

Представляет сведения о курсе для класса. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | Уникальный идентификатор для курса.         |
| description  | String | Описание курса.                |
| displayName  | String | Имя курса.                       |
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
