---
title: тип ресурса channelRenamedEventMessageDetail
description: Представляет сведения о сообщении события о переименовании канала.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e6f0b2ac19c9f51bbc0cc222bf81470509a2a265
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322623"
---
# <a name="channelrenamedeventmessagedetail-resource-type"></a>тип ресурса channelRenamedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о переименовании [канала.](../resources/channel.md)
Это сообщение создается  при обновлении имени канала.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|channelDisplayName|Строка|Обновленное имя **канала**.|
|channelId|Строка|Уникальный идентификатор **канала**.|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о переименовании **канала**](/graph/system-messages/#channel-renamed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
