---
title: Тип ресурса chatMessageMention
description: 'Представляет упоминание в объекте chatMessage. Упоминание может быть: на пользователя, группу, бот или канал. '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3557ad926ebad764d9ad734c372fd4c367d319e6
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819877"
---
# <a name="chatmessagemention-resource-type"></a>Тип ресурса chatMessageMention

Пространство имен: microsoft.graph

Представляет упоминание в [объекте chatMessage.](./chatmessage.md) Упоминанием может быть [пользователь,](user.md) [команда,](team.md)бот или [канал.](channel.md) 

В **объекте chatMessage,** содержащем одно или несколько упоминаний, свойство содержимого **сообщения** представляет сообщение чата в формате HTML. Он заключает **упоминание текста** каждого упоминания в `at` HTML-элементе с атрибутом, соответствующим `id` свойству **id** упоминания.

Например, сообщение чата содержит два упоминания со словом "Меган" и "Арк", соответственно. Свойство **содержимого в** теле определяет `at` элементы для двух упоминаний следующим образом:

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

В **свойстве содержимого** первый упоминание имеет АТРИБУТ HTML `id` 0. Соответствует свойству **id** первого экземпляра объекта **chatMessageMention,** которое также равно 0.

Второе `id` упоминание имеет атрибут 1, соответствующий свойству **id** второго экземпляра, значение 1.

Более полный контекст примера см. в ответах [на сообщения в виде списка.](/graph/api/channel-list-messagereplies?view=graph-rest-beta)

## <a name="properties"></a>Свойства

| Свойство| Тип|Описание|
|:---------------|:--------|:----------|
|id|Int32|Индекс сущности, упомянутого в **указанном объекте chatMessage.** Соответствует значению {index} с соответствующим `<at id="{index}">` тегом в тексте сообщения.|
|mentionText|строка|Строка, представляющая упоминание. Например, отображаемое имя пользователя, имя команды.|
|mentioned|[identitySet](identityset.md)|Указанный объект (пользователь, приложение, команда или канал).  Если это был канал или команда @mentioned, identitySet содержит свойство **беседы,** указывающее идентификатор команды или канала, и **свойство conversationIdentityType,** представляющее команду или канал.|


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
