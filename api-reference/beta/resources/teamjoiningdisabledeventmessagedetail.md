---
title: тип ресурса teamJoiningDisabledEventMessageDetail
description: Представляет сведения о сообщении события о присоединении группы к отключенным.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a509b23ef7239a9f8d75cc7895b2c4f7a53b50d4
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534415"
---
# <a name="teamjoiningdisabledeventmessagedetail-resource-type"></a>тип ресурса teamJoiningDisabledEventMessageDetail

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о присоединении группы к отключенным.
Это сообщение создается при отключении присоединения для группы.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamId|Строка|Уникальный идентификатор группы.|
## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamJoiningDisabledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamJoiningDisabledEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о присоединении группы к отключенным](/graph/system-messages/#team-joining-disabled)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)