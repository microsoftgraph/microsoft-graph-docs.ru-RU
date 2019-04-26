---
title: Тип ресурса Рискюсерхисторитем
description: ''
author: ''
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7143fffecee52747109674e81e5bfbd9860df7f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563057"
---
# <a name="riskyuserhistoryitem-resource-type"></a>Тип ресурса Рискюсерхисторитем

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>Свойства

| Свойство       | Тип    | Описание |
|:---------------|:--------|:------------|
| userId         | string  |             |
| initiatedBy    | bool    |             |
| activity       | [Рискусерактивити](riskuseractivity.md)| |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.riskyUserHistoryItem",
  "baseType": "microsoft.graph.riskyUser"
}-->

```json
{
    "userId": "string",
    "initiatedBy": "bool",
    "activity": {"@odata.type": "microsoft.graph.riskUserActivity"}
}
```


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
   
  ]
}
-->
