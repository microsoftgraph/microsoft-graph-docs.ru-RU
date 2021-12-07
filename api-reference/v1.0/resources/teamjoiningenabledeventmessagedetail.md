---
title: тип ресурса teamJoiningEnabledEventMessageDetail
description: Представляет сведения о сообщении события о присоединении к команде включено.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a024a2a7106661f16342bcffc9f832f1a25020c1
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322684"
---
# <a name="teamjoiningenabledeventmessagedetail-resource-type"></a>тип ресурса teamJoiningEnabledEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о присоединении [к команде](../resources/team.md) включено.
Это сообщение создается при включенном присоединении для **группы.**


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
  "@odata.type": "microsoft.graph.teamJoiningEnabledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamJoiningEnabledEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о **присоединении к** команде включен](/graph/system-messages/#team-joining-enabled)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
