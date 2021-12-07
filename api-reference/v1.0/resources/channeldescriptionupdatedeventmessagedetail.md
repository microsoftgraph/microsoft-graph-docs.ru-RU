---
title: channelDescriptionUpdatedEventMessageDetail resource type
description: Представляет сведения о сообщении события об обновленном описании канала.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7abd2a067d89a6c648d0d73e3060a3e4d91d5e9c
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322599"
---
# <a name="channeldescriptionupdatedeventmessagedetail-resource-type"></a>channelDescriptionUpdatedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об обновленном [описании](../resources/channel.md) канала.
Это сообщение создается при **обновлении** описания канала.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelDescription|Строка|Обновленное описание **канала**.|
|channelId|Строка|Уникальный идентификатор **канала**.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
  "channelId": "String",
  "channelDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события об обновленном **описании канала**](/graph/system-messages/#channel-description-updated)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
