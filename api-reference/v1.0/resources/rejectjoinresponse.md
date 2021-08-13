---
title: тип ресурса rejectJoinResponse
description: Содержит ответ на отклонение участника, который пытается присоединиться к собранию.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4a8868b07b84717176af01d70cdc6e86b671b8f4c0fe588db2c183909c252848
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163686"
---
# <a name="rejectjoinresponse-resource-type"></a>тип ресурса rejectJoinResponse

Пространство имен: microsoft.graph

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
