---
title: тип ресурса conditionalAccessFilter
description: Представляет фильтр в области политики.
localization_priority: Normal
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f5b14a3faa593453c88cc155f7e44348fcfda35
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082410"
---
# <a name="conditionalaccessfilter-resource-type"></a>тип ресурса conditionalAccessFilter

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет фильтр в области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| mode | filterMode | Режим использования для фильтра. Возможные значения: `include` или `exclude`. |
| правило | String | Синтаксис правил похож на тот, который используется для правил членства для групп в Azure AD. Подробные сведения см. [в правилах с несколькими выражениями](/azure/active-directory/enterprise-users/groups-dynamic-membership#rules-with-multiple-expressions) |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "mode",
    "rule"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessFilter",
  "baseType": null
}-->

```json
{
  "mode": "String",
  "rule": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessFilter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


