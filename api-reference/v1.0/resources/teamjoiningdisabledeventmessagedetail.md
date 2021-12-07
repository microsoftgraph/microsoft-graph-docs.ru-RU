---
title: тип ресурса teamJoiningDisabledEventMessageDetail
description: Представляет сведения о сообщении события о присоединении группы к отключенным.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a7082753265a6be3929f1b697e9e24f9b4e5f95a
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322660"
---
# <a name="teamjoiningdisabledeventmessagedetail-resource-type"></a>тип ресурса teamJoiningDisabledEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о [присоединении группы](../resources/team.md) к отключенным.
Это сообщение создается при отключении присоединения для **группы.**


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamId|String|Уникальный идентификатор **группы**.|
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
- [Пример ответа на сообщение события о **присоединении группы** к отключенным](/graph/system-messages/#team-joining-disabled)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
