---
title: Тип ресурса ПартиЦипантинфо
description: Содержит дополнительные свойства удостоверения участника
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568611"
---
# <a name="participantinfo-resource-type"></a>Тип ресурса ПартиЦипантинфо

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит дополнительные свойства удостоверения участника

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание  |
|:---------------|:------------------------------|:-------------|
| хищения       | [identitySet](identityset.md) | [Удостоверение](identityset.md) , связанное с этим участником. |
| languageId     | String                        | Строка языка и региональных параметров языка. |
| региональных         | String                        | Регион участника. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
