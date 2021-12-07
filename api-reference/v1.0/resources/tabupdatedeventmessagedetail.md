---
title: tabUpdatedEventMessageDetail resource type
description: Представляет сведения о сообщении события об обновленной вкладке.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 020adfcc34a8d2874e021d1b53441093c9f902f7
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322612"
---
# <a name="tabupdatedeventmessagedetail-resource-type"></a>tabUpdatedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об обновленной вкладке. Это сообщение создается при обновлении вкладки в [канале](../resources/channel.md) или [чате.](../resources/chat.md)


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|tabId|Строка|Уникальный идентификатор вкладки.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.tabUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tabUpdatedEventMessageDetail",
  "tabId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события об обновленной вкладке](/graph/system-messages/#tab-updated)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
