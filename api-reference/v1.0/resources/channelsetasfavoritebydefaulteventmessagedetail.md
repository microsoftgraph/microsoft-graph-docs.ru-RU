---
title: тип ресурса channelSetAsFavoriteByDefaultEventMessageDetail
description: Представляет сведения о сообщении события о канале, за наборе избранного по умолчанию.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 011414c5e0030bfcc0936c28de3a6bda1049052e
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322689"
---
# <a name="channelsetasfavoritebydefaulteventmessagedetail-resource-type"></a>тип ресурса channelSetAsFavoriteByDefaultEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о [канале,](../resources/channel.md) на который установлен `isFavoriteByDefault` флаг.

Канал **виден** всем участникам группы в  списке каналов под командой, [](../resources/team.md) если флаг `isFavoriteByDefault` `true` .


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelId|Строка|Уникальный идентификатор **канала**.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
  "channelId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о том, что **канал** по умолчанию установлен как любимый.](/graph/system-messages/#channel-set-as-favorite-by-default)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
