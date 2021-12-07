---
title: teamsAppInstalledEventMessageDetail resource type
description: Представляет сведения о сообщении о событии, установленном teamsApp.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8a68e75e98cce394554f165842ecb3b20ed075f9
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322696"
---
# <a name="teamsappinstalledeventmessagedetail-resource-type"></a>teamsAppInstalledEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения о сообщении о событии, [установленном teamsApp.](../resources/teamsApp.md)
Это сообщение создается при установке **teamsApp** в [канале,](../resources/channel.md) [чате](../resources/chat.md)или [команде.](../resources/team.md)


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
- [Пример ответа на сообщение о **событии, установленном teamsApp**](/graph/system-messages/#teams-app-installed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
