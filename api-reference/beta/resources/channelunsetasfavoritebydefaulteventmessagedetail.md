---
title: тип ресурса channelUnsetAsFavoriteByDefaultEventMessageDetail
description: Представляет сведения о сообщении события о канале, расстановленном как любимый по умолчанию.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a30aecbd82d7b6a0ea7d6043cf1cfa832d40ae56
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535784"
---
# <a name="channelunsetasfavoritebydefaulteventmessagedetail-resource-type"></a>тип ресурса channelUnsetAsFavoriteByDefaultEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о канале, что флаг "isFavoriteByDefault" неустановлен.
Канал больше не отображается для всех членов команды в списке каналов под командой, если у него есть флаг "isFavoriteByDefault", задаваемый ложным.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelId|Строка|Уникальный идентификатор канала.|
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
- [Пример ответа на сообщение события о том, что канал по умолчанию не замечен как любимый.](/graph/system-messages/#channel-unset-as-favorite-by-default)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)