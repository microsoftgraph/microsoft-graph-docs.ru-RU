---
title: Тип ресурса Чатмессажементион
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть у пользователя, группы, ленты или канала. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b6a63380475be8bd0e669851f7e760a9f645d18d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064283"
---
# <a name="chatmessagemention-resource-type"></a>Тип ресурса Чатмессажементион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет упоминание в объекте [chatMessage](chatmessage.md) . Упоминание может быть у [пользователя](user.md), [группы](team.md), ленты или [канала](channel.md). 

В объекте **chatMessage** , содержащем одно или несколько упоминаний, свойство **Content** текста сообщения представляет сообщение чата в HTML. Он заключает **ментионтекст** каждого упоминания в `at` элементе HTML с `id` атрибутом, соответствующим свойству **ID** упомянутого упоминания.

Например, сообщение чата содержит два упомянутых элемента с текстом "Меган" и "Алекс" соответственно. Его свойство Body свойства **Content** определяет `at` элементы для двух упомянутых ниже элементов.

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

В свойстве **Content** первое упоминание имеет `id` атрибут HTML 0. Это соответствует свойству **ID** этого первого экземпляра **чатмессажементион**, которое также равно 0.

Второе упоминание имеет `id` атрибут 1, совпадающий со свойством **ID** второго экземпляра, который равен 1.

Полный контекст этого примера приведен в разделе [список ответов на сообщения канала](../api/channel-list-messagereplies.md#example).

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|id|Int32|Индекс объекта, упоминаемого в заданном **chatMessage**. Соответствует значению {index} в соответствующем `<at id="{index}">` теге в тексте сообщения.|
|ментионтекст|string|Строка, используемая для представления упоминания. Например, отображаемое имя пользователя, имя группы.|
|котором|[identitySet](identityset.md)|Упоминаемая сущность (пользователь, приложение, группа или канал).  Если это канал или группа, @mentioned, Identity содержит свойство **CONVERSATION** , предоставляющее идентификатор команды или канала, и свойство **конверсатионидентититипе** , которое представляет группу или канал.|


## <a name="json-representation"></a>Представление в формате JSON

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


