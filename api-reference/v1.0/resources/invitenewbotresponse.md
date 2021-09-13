---
title: тип ресурса inviteNewBotResponse
description: Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cca303fff854fddff56f6bc8ffd30160f390401c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084407"
---
# <a name="invitenewbotresponse-resource-type"></a>тип ресурса inviteNewBotResponse

Пространство имен: microsoft.graph

Содержит ответ на запрос о повторном отправлении уведомления о присоединении участника в качестве входящих вызовов в нужное расположение.

## <a name="properties"></a>Свойства

| Свойство         | Тип                            | Описание                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| inviteUri        | Строка                          | URI для получения нового уведомления о входящих вызовах.                                                                                                                |

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
