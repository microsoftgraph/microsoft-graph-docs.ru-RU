---
title: тип ресурса inviteNewBotResponse
description: Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3811c1b5aa6fe21a361cd371ab0b39e6ea00c7b1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447522"
---
# <a name="invitenewbotresponse-resource-type"></a>тип ресурса inviteNewBotResponse

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
