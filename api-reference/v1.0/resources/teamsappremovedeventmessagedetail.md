---
title: teamsAppRemovedEventMessageDetail resource type
description: Представляет сведения об удалении сообщения о событиях teamsApp.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2077abe27aec8f81f690f30b5bbe7345093a54af
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322582"
---
# <a name="teamsappremovedeventmessagedetail-resource-type"></a>teamsAppRemovedEventMessageDetail resource type

Пространство имен: microsoft.graph

Представляет сведения об удалении [сообщения о событиях teamsApp.](../resources/teamsApp.md)
Это сообщение создается, когда **teamsApp** удаляется из [канала,](../resources/channel.md) [чата](../resources/chat.md)или [команды.](../resources/team.md)


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
- [Пример ответа на сообщение о **событии об удалении teamsApp**](/graph/system-messages/#teams-app-removed)
- Дополнительные сведения о других типах событий см. в [сообщении System.](/graph/system-messages)
