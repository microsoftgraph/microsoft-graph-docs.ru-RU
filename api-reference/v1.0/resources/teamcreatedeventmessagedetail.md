---
title: тип ресурса teamCreatedEventMessageDetail
description: Представляет сведения о сообщении события о созданной команде.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c60ceda4f89832671700ed929bc80b5cb0078edf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322587"
---
# <a name="teamcreatedeventmessagedetail-resource-type"></a>тип ресурса teamCreatedEventMessageDetail

Пространство имен: microsoft.graph

Представляет сведения о сообщении события о созданной [команде.](../resources/team.md)
Это сообщение создается, **когда создается** команда.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamDescription|Строка|Описание для **команды**.|
|teamDisplayName|Строка|Отображение имени **команды.**|
|teamId|Строка|Уникальный идентификатор **группы**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamCreatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamCreatedEventMessageDetail",
  "teamId": "String",
  "teamDisplayName": "String",
  "teamDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение события о созданной **команде**](/graph/system-messages/#team-created)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
