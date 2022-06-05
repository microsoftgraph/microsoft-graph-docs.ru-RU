---
title: Тип ресурса educationFeedbackResourceOutcome
description: Представляет отзыв об объекте educationOutcome в виде документа.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0cad7a6e8c2f0527dd89ce624fac5652c6ac544b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65900570"
---
# <a name="educationfeedbackresourceoutcome-resource-type"></a>Тип ресурса educationFeedbackResourceOutcome

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет отзыв об [объекте educationOutcome](educationoutcome.md) в виде документа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание educationFeedbackResourceOutcome](../api/educationfeedbackresourceoutcome-post-outcomes.md) | [educationOutcome](educationoutcome.md) | Создайте ресурс [обратной связи для](../resources/educationfeedbackresourceoutcome.md) отправки. |
| [Удаление educationFeedbackResourceOutcome](../api/educationfeedbackresourceoutcome-delete.md) | Нет | Удаление ресурса [обратной связи](../resources/educationfeedbackresourceoutcome.md) из отправки. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|feedbackResource|[educationResource](educationresource.md)|Фактический ресурс обратной связи.|
|id|Строка|Уникальный идентификатор для **educationFeedbackResourceOutcome**.|
|resourceStatus|educationFeedbackResourceOutcomeStatus|Состояние ресурса обратной связи. Возможные значения: , , , `published`, и . `failedPublish``unknownFutureValue``pendingPublish``notPublished`|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackResourceOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedbackResource": {"@odata.type": "microsoft.graph.educationResource"},
  "id": "String (identifier)",
  "resourceStatus": {"@odata.type": "microsoft.graph.educationFeedbackResourceOutcomeStatus"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2022-05-05 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackResourceOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
