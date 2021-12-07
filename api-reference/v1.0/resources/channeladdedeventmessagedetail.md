---
title: тип ресурса channelAddedEventMessageDetail
description: Представляет сведения о сообщении события о канале, добавленном в команду.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a93e6f24992d361f92eb0831f8334a225fc95bf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322635"
---
# <a name="channeladdedeventmessagedetail-resource-type"></a>тип ресурса channelAddedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о [канале,](../resources/channel.md) добавленном в [команду.](../resources/team.md)
Это сообщение создается при добавлении **стандартного** канала в **команду.**


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelDisplayName|Строка|Отображение имени **канала**.|
|channelId|Строка|Уникальный идентификатор **канала**.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о **канале,** добавленном в **команду**](/graph/system-messages/#channel-added)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
