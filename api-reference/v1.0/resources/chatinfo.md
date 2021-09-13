---
title: тип ресурса chatInfo
description: Сведения о сообщении в Microsoft Teams.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc548c9f107232368b43aaeb154db2cf5e2cc517
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109432"
---
# <a name="chatinfo-resource-type"></a>тип ресурса chatInfo

Пространство имен: microsoft.graph

Это содержит сведения, связанные с Microsoft Teams собраниями.

## <a name="properties"></a>Свойства

| Свойство            | Тип    | Описание|
|:--------------------|:--------|:-----------|
| messageId           | Строка  | Уникальный идентификатор сообщения в Microsoft Teams канале. |
| replyChainMessageId | Строка  | ID ответного сообщения. |
| threadId            | String  | Уникальный идентификатор для потока в Microsoft Teams. |

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

