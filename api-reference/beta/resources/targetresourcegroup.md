---
title: Тип ресурса targetResourceGroup
description: 'Указывает тип группы, которая изменилась из-за загрузки аудита. Содержит значения, как объединенные группам и Azure AD '
ms.openlocfilehash: 3427f2401a0e93767f0c563842be323f66d9f21b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078090"
---
# <a name="targetresourcegroup-resource-type"></a>Тип ресурса targetResourceGroup
Указывает тип группы, которая изменилась из-за загрузки аудита. Содержит значения, как объединенные группам и Azure AD 



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|groupType|String| Возможные значения: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceGroup"
}-->

```json
{
  "groupType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->