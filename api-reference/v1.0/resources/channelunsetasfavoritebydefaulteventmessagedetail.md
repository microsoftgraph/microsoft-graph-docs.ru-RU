---
title: тип ресурса channelUnsetAsFavoriteByDefaultEventMessageDetail
description: Представляет сведения о сообщении события о канале, расстановленном как любимый по умолчанию.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4f9dab965db79fe08086af3327d727ac97713f3f
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322642"
---
# <a name="channelunsetasfavoritebydefaulteventmessagedetail-resource-type"></a>тип ресурса channelUnsetAsFavoriteByDefaultEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о [канале,](../resources/channel.md) который не `isFavoriteByDefault` засечен флагом.

Канал **больше** не отображается для всех членов группы  в списке каналов под командой, [](../resources/team.md) если флаг `isFavoriteByDefault` `false` .

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
  "@odata.type": "microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
  "channelId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о том, что **канал по** умолчанию не замечен как любимый.](/graph/system-messages/#channel-unset-as-favorite-by-default)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
