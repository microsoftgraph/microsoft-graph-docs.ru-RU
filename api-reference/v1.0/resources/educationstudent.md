---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 590ff35d318114f054daf429157165674157076d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123645"
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

## <a name="relationships"></a>Отношения

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
