---
title: тип ресурса teamArchivedEventMessageDetail
description: Представляет сведения о сообщении события о архивной группе.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3badd933d5ea0c985c0b245a4afc8a6e7b061ff2
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322648"
---
# <a name="teamarchivedeventmessagedetail-resource-type"></a>тип ресурса teamArchivedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о архивной [группе.](../resources/team.md)
Это сообщение создается при **архивировании** группы.


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
  "@odata.type": "microsoft.graph.teamArchivedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamArchivedEventMessageDetail",
  "teamId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о группе **архивов**](/graph/system-messages/#team-archived)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
