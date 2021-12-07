---
title: тип ресурса channelDeletedEventMessageDetail
description: Представляет сведения о сообщении события о канале, удаленном из группы.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 99a009ac2fd967a8ebcc3a7a688f34e0f84cdfde
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322629"
---
# <a name="channeldeletedeventmessagedetail-resource-type"></a>тип ресурса channelDeletedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о [канале,](../resources/channel.md) удаленном из [группы.](../resources/team.md)
Это сообщение создается  при удалении стандартного канала из **группы.**


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
- [Пример ответа на сообщение события о **канале,** удаленном из **группы.**](/graph/system-messages/#channel-deleted)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
