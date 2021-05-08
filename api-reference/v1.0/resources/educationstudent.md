---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b0e154beb5b8133c69392af8fa9611263c68945
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231852"
---
# <a name="educationstudent-resource-type"></a>Тип ресурса educationStudent

Пространство имен: microsoft.graph

Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.

## <a name="properties"></a>Свойства

| Свойство       | Тип            | Описание                                                               |
| :------------- | :-------------- | :------------------------------------------------------------------------ |
| birthDate      | Date            | Дата рождения учащегося.                                                |
| externalId     | String          | Идентификатор учащегося в исходной системе.                                   |
| gender         | educationGender | Допустимые значения: `female`, `male`, `other`, `unknownFutureValue`. |
| оценка          | String          | Текущий уровень оценок учащегося.                                       |
| graduationYear | String          | Год выпуска учащегося из школы.                           |
| studentNumber  | String          | Student Number.                                                           |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "DateTimeOffset",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```
