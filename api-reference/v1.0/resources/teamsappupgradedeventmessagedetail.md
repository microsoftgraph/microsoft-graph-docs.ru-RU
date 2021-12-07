---
title: teamsAppUpgradedEventMessageDetail type
description: Представляет сведения о сообщении события об обновлении teamsApp.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 119b32650be32612e90134ff87e593e7132b9741
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322575"
---
# <a name="teamsappupgradedeventmessagedetail-resource-type"></a>teamsAppUpgradedEventMessageDetail type

Пространство имен: microsoft.graph

Представляет сведения о сообщении события об [обновлении teamsApp.](../resources/teamsApp.md)
Это сообщение создается при обновлении **teamsApp** в [канале,](../resources/channel.md) [чате](../resources/chat.md)или [команде.](../resources/team.md)


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
- [Пример ответа на сообщение о событии **об обновлении teamsApp**](/graph/system-messages/#teams-app-upgraded)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
