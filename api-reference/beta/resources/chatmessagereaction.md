---
title: Тип ресурса Чатмессажереактион
description: 'Представляет реакцию на объект chatMessage. '
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 33fe5a881d05b2ac2bc86e97e11b00c3465a8c09
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709427"
---
# <a name="chatmessagereaction-resource-type"></a>Тип ресурса Чатмессажереактион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет реакцию на объект [chatMessage](chatmessage.md) . 

Сущность типа `chatMessageReaction` возвращается в составе интерфейса [сообщения канала Get](../api/channel-get-message.md) в виде части объекта [chatMessage](chatmessage.md) .

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|Реактионтипе|String|Планируемые значения включают: <br><ul><li>В данном случае, как и сообщение, в этом случае используется пустое содержимое.</li><li>Эмодзи, реакция на эмодзи. Для содержимого задано значение Юникод для эмодзи.</li><li>Label — содержимое задается в виде строки в метке.</li></ul>|
|user|[identitySet](identityset.md)|Пользователь, который реагировал на сообщение.|

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
  "user": {"@odata.type": "microsoft.graph.identitySet"}
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
