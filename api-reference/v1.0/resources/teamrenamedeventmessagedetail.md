---
title: teamRenamedEventMessageDetail resource type
description: Представляет сведения о сообщении события о переименованной команде.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c1569be468116d539d0144519d0225975abf004b
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322563"
---
# <a name="teamrenamedeventmessagedetail-resource-type"></a>teamRenamedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о переименованной [команде.](../resources/team.md)
Это сообщение создается при **обновлении** имени команды.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamDisplayName|String|Обновленное имя **команды.**|
|teamId|String|Уникальный идентификатор **группы**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamRenamedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о переименованной **команде**](/graph/system-messages/#team-renamed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
