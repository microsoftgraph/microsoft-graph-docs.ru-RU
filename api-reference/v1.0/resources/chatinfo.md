---
title: Тип ресурса Чатинфо
description: Сведения о сообщении в Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ee55fc2f9321a5b16c3a24ec330f5966472f4f9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059175"
---
# <a name="chatinfo-resource-type"></a>Тип ресурса Чатинфо

Пространство имен: microsoft.graph

Содержит сведения, связанные с собраниями Microsoft Teams.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| messageId           | String  | Уникальный идентификатор сообщения в канале Microsoft Teams. |
| репличаинмессажеид | String  | Идентификатор ответного сообщения. |
| Tидентификатор            | String  | Уникальный идентификатор потока в Microsoft Teams. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

