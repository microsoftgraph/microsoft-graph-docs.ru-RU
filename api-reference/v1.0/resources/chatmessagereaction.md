---
title: тип ресурса chatMessageReaction
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: fd94315fef0d11eb5dc54fb592dc7de01f912757
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208927"
---
# <a name="chatmessagereaction-resource-type"></a>тип ресурса chatMessageReaction

Пространство имен: microsoft.graph

Представляет реакцию на [объект chatMessage.](chatmessage.md) 

Объект типа возвращается в рамках API сообщения get channel, как часть `chatMessageReaction` [сущности chatMessage.](chatmessage.md) [](../api/chatmessage-get.md)

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|reactionType|String|Поддерживаемые значения `like` : , , , , `angry` `sad` `laugh` `heart` `surprised` . |
|user|[chatMessageReactionIdentitySet](chatmessagereactionidentityset.md)|Пользователь, реагирувший на сообщение.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


