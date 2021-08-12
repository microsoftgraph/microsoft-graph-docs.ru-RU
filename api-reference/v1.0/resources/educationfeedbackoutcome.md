---
title: тип ресурса educationFeedbackOutcome
description: EducationOutcome, который дает обратную связь в виде текста.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5d3e28fa7ee3157a1cf05b2fcf4818878e292702738c5b3e813bccbf39caff9b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146925"
---
# <a name="educationfeedbackoutcome-resource-type"></a>тип ресурса educationFeedbackOutcome

Пространство имен: microsoft.graph

Представляет обратную связь по [объекту educationOutcome](educationoutcome.md) в виде текста. 

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|feedback|[educationFeedback](educationfeedback.md)|Письменные отзывы преподавателя для учащегося.|
|publishedFeedback|[educationFeedback](educationfeedback.md)|Копия свойства обратной связи, которая сделана при отсвойке класса учащемуся.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

