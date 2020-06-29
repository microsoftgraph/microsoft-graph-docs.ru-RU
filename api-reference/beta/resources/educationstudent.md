---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e64899cf56140246373c36428518ebd28bb136c7
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909725"
---
# <a name="educationstudent-resource-type"></a>Тип ресурса educationStudent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.

> [!IMPORTANT]
> При использовании делегированных областей разрешений Graph будет возвращать только `externalId` Свойства. Для всех остальных свойств требуются области применения.

## <a name="properties"></a>Свойства

| Свойство       | Тип            | Описание                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| birthDate      | Date            | Дата рождения учащегося.                      |
| externalId     | String          | Идентификатор учащегося в исходной системе.         |
| gender         | едукатионжендер | Возможные значения: `female`, `male`, `other`. |
| оценка          | String          | Текущий уровень оценок учащегося.             |
| graduationYear | String          | Год выпуска учащегося из школы. |
| studentNumber  | String          | Student Number.                                 |

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
