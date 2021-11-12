---
title: teamsAppRemovedEventMessageDetail resource type
description: Представляет сведения об удалении сообщения о событиях teamsApp.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b08519771e90cf52a2701898a0cea56d7e049aa3
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890971"
---
# <a name="teamsappremovedeventmessagedetail-resource-type"></a>teamsAppRemovedEventMessageDetail resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события об удалении **teamsApp.**
Это сообщение создается, когда **teamsApp** удаляется из канала, чата или группы.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamsAppDisplayName|String|Отображение имени **teamsApp**.|
|teamsAppId|String|Уникальный идентификатор **teamsApp**.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsAppRemovedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppRemovedEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии об удалении teamsApp](/graph/system-messages/#teams-app-removed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
