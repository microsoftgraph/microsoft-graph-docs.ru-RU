---
title: teamsAppUpgradedEventMessageDetail type
description: Представляет сведения о сообщении события об обновлении teamsApp.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4bca8bbb7c218333d72cb290e508b352fd977f2d
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535807"
---
# <a name="teamsappupgradedeventmessagedetail-resource-type"></a>teamsAppUpgradedEventMessageDetail type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении события об обновлении teamsApp.
Это сообщение создается при обновлении teamsApp в канале, чате или команде.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamsAppDisplayName|Строка|Отображение имени teamsApp.|
|teamsAppId|Строка|Уникальный идентификатор teamsApp.|

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