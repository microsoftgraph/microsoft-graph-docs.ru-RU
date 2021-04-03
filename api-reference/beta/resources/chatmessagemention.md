---
title: тип ресурса chatMessageMention
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть для пользователя, команды, бота или канала. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7671f438544392ca9c8b60523c910e82873c848b
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582559"
---
# <a name="chatmessagemention-resource-type"></a>тип ресурса chatMessageMention

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет упоминание в [объекте chatMessage.](chatmessage.md) Упоминание может быть для пользователя, [команды,](user.md)бота или [канала](channel.md). [](team.md) 

В **объекте chatMessage,** который содержит одно или  несколько упоминаний, свойство контента тела сообщения представляет сообщение чата в HTML. В него **заключено упоминание Каждого** упоминания в элементе HTML с атрибутом, соответствующим свойству `at` `id` **id** упоминания.

В качестве примера, сообщение чата содержит два упоминания, с текстом упоминания "Меган" и "Алекс" соответственно. Свойство **контента** тела указывает элементы для `at` этих двух упоминаний следующим образом:

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

В **свойстве контента** первое упоминание имеет htmL-атрибут `id` 0. Это соответствует свойству **id** этого первого экземпляра **chatMessageMention,** которое также является 0.

Второе упоминание имеет атрибут 1, совпадающий с свойством `id` **id** второго экземпляра, которое является 1.

Более полный контекст примера см. в списке [ответов на сообщения канала.](../api/chatmessage-list-replies.md#example)

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Int32|Индекс сущности, упоминаемой в указанном **chatMessage.** Соответствует значению {index} в соответствующем `<at id="{index}">` теге в теле сообщения.|
|mentionText|string|Строка, используемая для представления упоминания. Например, имя отображения пользователя, имя команды.|
|упомянутый|[identitySet](identityset.md)|Упомянутая сущность (пользователь, приложение, команда или канал).  Если это был канал или команда, @mentioned, identitySet  содержит свойство разговоров, дающий идентификатор команды/канала, и свойство **conversationIdentityType,** которое представляет команду или канал.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


