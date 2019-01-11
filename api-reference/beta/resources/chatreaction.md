---
title: Тип ресурса chatMessageReaction
description: 'Представляет реакцию на chatMessage сущности. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810068"
---
# <a name="chatmessagereaction-resource-type"></a>Тип ресурса chatMessageReaction

Представляет реакцию на [chatMessage](chatmessage.md) сущности. 

Сущность типа `chatMessageReaction` возвращается как часть [получить сообщения](../api/channel-get-message.md) API, как часть [chatMessage](chatmessage.md) сущности.

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
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
