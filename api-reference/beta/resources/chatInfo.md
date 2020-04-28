---
title: Тип ресурса Чатинфо
description: Содержит сведения, связанные с собраниями Microsoft Teams.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8602301af0de458f07ab5a9c0af00ec8578c3a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507735"
---
# <a name="chatinfo-resource-type"></a>Тип ресурса Чатинфо

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
