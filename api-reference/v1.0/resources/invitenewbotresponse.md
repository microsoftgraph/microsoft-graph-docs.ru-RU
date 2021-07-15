---
title: тип ресурса inviteNewBotResponse
description: Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 675b7cd1df35b25e3414f36a4dd04e389e05b192
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430188"
---
# <a name="invitenewbotresponse-resource-type"></a>тип ресурса inviteNewBotResponse

Пространство имен: microsoft.graph

Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.

## <a name="properties"></a>Свойства

| Свойство         | Тип                            | Описание                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| inviteUri        | String                          | URI для получения нового уведомления о входящих вызовах.                                                                                                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.inviteNewBotResponse"
}-->
```json
{
  "inviteUri": "uri" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inviteNewBotResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
