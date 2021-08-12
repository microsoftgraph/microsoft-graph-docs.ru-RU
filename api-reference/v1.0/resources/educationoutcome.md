---
title: тип ресурсов educationOutcome
description: Результат классификации назначения.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c393b5b324112ce268b310ef5981f335717594edf1d7cfd751e243cceeb633c7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212123"
---
# <a name="educationoutcome-resource-type"></a>тип ресурсов educationOutcome

Пространство имен: microsoft.graph

Результат классификации назначения. 

Это базовый класс; производными типами являются [educationFeedbackOutcome,](educationfeedbackoutcome.md) [educationPointsOutcome](educationpointsoutcome.md)и [educationRubricOutcome.](educationrubricoutcome.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление educationOutcome](../api/educationoutcome-update.md) | [educationOutcome](educationoutcome.md) | Обновление объекта educationOutcome. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

