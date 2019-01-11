---
title: Тип ресурса targetResourceGroup
description: 'Указывает тип группы, которая изменилась из-за загрузки аудита. Содержит значения, как объединенные группам и Azure AD '
localization_priority: Normal
ms.openlocfilehash: 2cc7e0adb1a93394b64375d05dfb6a6e349bac55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851186"
---
# <a name="targetresourcegroup-resource-type"></a>Тип ресурса targetResourceGroup
Указывает тип группы, которая изменилась из-за загрузки аудита. Содержит значения, как объединенные группам и Azure AD 



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|groupType|Строка| Возможные значения: `unifiedGroups`, `azureAD`, `unknownFutureValue`.|

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
