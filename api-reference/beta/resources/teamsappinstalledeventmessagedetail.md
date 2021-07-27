---
title: teamsAppInstalledEventMessageDetail resource type
description: Представляет сведения о сообщении о событии, установленном teamsApp.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 04ed2f02c64d5339f0343445614ef7cf7a069f2a
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535811"
---
# <a name="teamsappinstalledeventmessagedetail-resource-type"></a>teamsAppInstalledEventMessageDetail resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о сообщении о событии, установленном teamsApp.
Это сообщение создается при установке teamsApp в канале, чате или команде.


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
  "@odata.type": "microsoft.graph.teamsAppInstalledEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppInstalledEventMessageDetail",
  "teamsAppId": "String",
  "teamsAppDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>См. также
- [Пример ответа на сообщение о событии, установленном teamsApp](/graph/system-messages/#teams-app-installed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)