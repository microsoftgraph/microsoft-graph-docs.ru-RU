---
title: тип ресурса channelSetAsFavoriteByDefaultEventMessageDetail
description: Представляет сведения о сообщении события о канале, за наборе избранного по умолчанию.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35ddf629e82b55bb3ab475d65d6078e4607392a1
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535787"
---
# <a name="channelsetasfavoritebydefaulteventmessagedetail-resource-type"></a>тип ресурса channelSetAsFavoriteByDefaultEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о канале, задаваемом флагом "isFavoriteByDefault".
Канал виден всем участникам группы в списке каналов под командой, если он имеет флаг "isFavoriteByDefault", установленный для true.


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
- [Пример ответа на сообщение события о том, что канал по умолчанию установлен как любимый.](/graph/system-messages/#channel-set-as-favorite-by-default)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)