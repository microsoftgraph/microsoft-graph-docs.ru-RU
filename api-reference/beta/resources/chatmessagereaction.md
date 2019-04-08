---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481386"
---
# <a name="chatmessagereaction-resource-type"></a>Тип ресурса Чатмессажереактион

Представляет реакцию на объект [chatMessage](chatmessage.md) . 

Сущность типа `chatMessageReaction` возвращается в составе API [сообщений канала](../api/channel-get-message.md) в составе объекта [chatMessage](chatmessage.md) .

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Реактионтипе|string| Тип реакции. Планируемые значения включают: <br><ul><li>В данном случае, как и сообщение, в этом случае используется пустое содержимое.</li><li>Эмодзи, реакция на эмодзи. Для содержимого задано значение Юникод для эмодзи.</li><li>Label — содержимое задается в виде строки в метке.</li></ul>|
|createdDateTime|dateTimeOffset|Метка времени в формате UTC для корневого сообщения в формате ISO-8601.|
|user|identitySet|Пользователь, который реагировал на сообщение.|

## <a name="json-representation"></a>Представление в формате JSON

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
