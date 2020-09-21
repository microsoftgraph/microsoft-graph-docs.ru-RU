---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2eae690076553090dbd32f46f0b777a998b615d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979541"
---
# <a name="educationteacher-resource-type"></a>Тип ресурса educationTeacher

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.

> [!IMPORTANT]
> При использовании делегированных областей разрешений Graph будет возвращать только `externalId` Свойства. Для всех остальных свойств требуются области применения.

## <a name="properties"></a>Свойства

| Свойство      | Тип   | Описание                                  |
| :------------ | :----- | :------------------------------------------- |
| externalId    | String | Идентификатор преподавателя во внешней исходной системе. |
| teacherNumber | String | Номер преподавателя.                              |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


