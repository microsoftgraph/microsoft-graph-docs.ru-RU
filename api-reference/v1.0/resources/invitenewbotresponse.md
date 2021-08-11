---
title: тип ресурса inviteNewBotResponse
description: Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 79f7f4b00aa8e549090ec06b5a22b522b9d966af86df02caf40762b0f661246a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189480"
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
