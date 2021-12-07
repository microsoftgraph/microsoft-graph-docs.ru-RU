---
title: teamDescriptionUpdatedEventMessageDetail resource type
description: Представляет сведения о сообщении события об обновленном описании группы.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8d7fbb900fb302f70a174d5549cba8feec740084
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322544"
---
# <a name="teamdescriptionupdatedeventmessagedetail-resource-type"></a>teamDescriptionUpdatedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об обновленном [описании](../resources/team.md) группы.
Это сообщение создается  при обновлении описания группы.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamDescription|String|Обновленное описание **для группы**.|
|teamId|String|Уникальный идентификатор **группы**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamDescriptionUpdatedEventMessageDetail",
  "teamId": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии об обновленном **описании** группы](/graph/system-messages/#team-description-updated)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
