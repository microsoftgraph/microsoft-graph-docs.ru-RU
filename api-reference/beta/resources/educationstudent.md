---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9b8f2de9f3b40a72aab7f9273b9b4fc30594059b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500767"
---
# <a name="educationstudent-resource-type"></a>Тип ресурса educationStudent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|birthDate|Date| Дата рождения учащегося.|
|externalId|String| Идентификатор учащегося в исходной системе.|
|gender|едукатионжендер| Возможные значения: `female`, `male`, `other`.|
|оценка|String|Текущий уровень оценок учащегося.|
|graduationYear|String| Год выпуска учащегося из школы.|
|studentNumber|String| Student Number.|

## <a name="json-representation"></a>Представление JSON

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
