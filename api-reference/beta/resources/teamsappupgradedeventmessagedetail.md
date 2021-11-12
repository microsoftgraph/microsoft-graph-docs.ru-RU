---
title: teamsAppUpgradedEventMessageDetail type
description: Представляет сведения о сообщении события об обновлении teamsApp.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1ab9353c2d64073b21ebc7551ac30a8dad6d8525
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890572"
---
# <a name="teamsappupgradedeventmessagedetail-resource-type"></a>teamsAppUpgradedEventMessageDetail type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события о обновлении **teamsApp.**
Это сообщение создается при обновлении **teamsApp** в канале, чате или команде.


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
  "@odata.type": "microsoft.graph.teamsAppUpgradedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppUpgradedEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии об обновлении teamsApp](/graph/system-messages/#teams-app-upgraded)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
