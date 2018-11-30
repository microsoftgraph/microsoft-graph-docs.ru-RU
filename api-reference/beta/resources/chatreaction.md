---
title: Тип ресурса chatMessageReaction
description: 'Представляет реакцию на chatMessage сущности. '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082519"
---
# <a name="chatmessagereaction-resource-type"></a>Тип ресурса chatMessageReaction

Представляет реакцию на [chatMessage](chatmessage.md) сущности. 

Сущность типа `chatMessageReaction` возвращается как часть [получить сообщения](../api/channel-get-message.md) API, как часть [chatMessage](chatmessage.md) сущности.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|reactionType|string| Тип реакции. Запланированные значения: <br><ul><li>Как - как сообщение, контент не задан в этом случае.</li><li>Emoji - Emoji реакции. Содержимое задано значение Юникод из emoji.</li><li>Подпись — содержимое задано значение строки в метку.</li></ul>|
|createdDateTime|dateTimeOffset|Метка времени UTC корневой сообщения в формате ISO 8601.|
|user|identitySet|Пользователь, отреагировало на сообщение.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
