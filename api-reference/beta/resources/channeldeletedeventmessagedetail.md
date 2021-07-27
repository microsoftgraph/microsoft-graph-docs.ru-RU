---
title: тип ресурса channelDeletedEventMessageDetail
description: Представляет сведения о сообщении события о канале, удаленном из группы.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0bfbba7d754ec7c40e966315b51122ce8086f356
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535791"
---
# <a name="channeldeletedeventmessagedetail-resource-type"></a>тип ресурса channelDeletedEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о канале, удаленном из группы.
Это сообщение создается при удалении стандартного канала из группы.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelDisplayName|Строка|Отображение имени канала.|
|channelId|Строка|Уникальный идентификатор канала.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelDeletedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelDeletedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о канале, удаленном из группы.](/graph/system-messages/#channel-deleted)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)