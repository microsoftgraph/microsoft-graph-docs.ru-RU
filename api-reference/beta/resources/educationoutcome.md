---
title: Тип ресурса Едукатионауткоме
description: Результат ступенчатого задания
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7ad67435af93eff4464fa585fa5c54d5fa3f4511
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501481"
---
# <a name="educationoutcome-resource-type"></a>Тип ресурса Едукатионауткоме

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Результат ступенчатого присваивания. Это базовый класс; производные типы: [едукатионфидбаккауткоме](educationfeedbackoutcome.md), [едукатионпоинтсауткоме](educationpointsoutcome.md)и [едукатионрубрикауткоме](educationrubricoutcome.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Обновление Едукатионауткоме](../api/educationoutcome-update.md) | [едукатионауткоме](educationoutcome.md) | Обновление объекта Едукатионауткоме. |

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "baseType": "",
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