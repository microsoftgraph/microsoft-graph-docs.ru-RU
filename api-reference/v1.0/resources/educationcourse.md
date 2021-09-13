---
title: тип ресурса educationCourse
description: Представляет сведения о курсе для класса.
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1b0345e6be308a175fbb14ab618fcf66564f45f9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036713"
---
# <a name="educationcourse-resource-type"></a>тип ресурса educationCourse

Пространство имен: microsoft.graph

Представляет сведения о курсе для класса. Используется в [educationClass](educationclass.md).

## <a name="properties"></a>Свойства

| Свойство     | Тип   | Описание                               |
| :----------- | :----- | :---------------------------------------- |
| courseNumber | String | Уникальный идентификатор для курса.         |
| description  | Строка | Описание курса.                |
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
