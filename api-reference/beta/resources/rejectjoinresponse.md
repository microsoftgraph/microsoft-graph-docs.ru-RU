---
title: тип ресурса rejectJoinResponse
description: Содержит ответ на отклонение участника, который пытается присоединиться к собранию.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4219a8093c1914d65f3f36ea1a3b700b47af000c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447330"
---
# <a name="rejectjoinresponse-resource-type"></a>тип ресурса rejectJoinResponse

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит ответ на отклонение участника, который пытается присоединиться к собранию.

Это имеет тот же эффект, что и отклонение уведомления о входящих вызовах политики с помощью метода [отклонить вызов.](../api/call-reject.md) Бот будет по-прежнему получать уведомление о присоединении участника к новому пользователю до тех пор, пока его емкость не будет достигнута.

## <a name="properties"></a>Свойства

| Свойство         | Тип                            | Описание                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| reason           | String                          | Причина отказа. Возможные значения: `None`, `Busy` и `Forbidden`.                                                                                     |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.rejectJoinResponse"
}-->
```json
{
  "reason": "None | Busy | Forbidden" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rejectJoinResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
