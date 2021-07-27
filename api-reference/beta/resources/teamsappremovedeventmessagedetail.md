---
title: teamsAppRemovedEventMessageDetail resource type
description: Представляет сведения об удалении сообщения о событиях teamsApp.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 24d080e77d679e0e12970be2b78ea3af7b4d6668
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535808"
---
# <a name="teamsappremovedeventmessagedetail-resource-type"></a>teamsAppRemovedEventMessageDetail resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об удалении сообщения о событиях teamsApp.
Это сообщение создается, когда teamsApp удаляется из канала, чата или группы.


Наследует [от eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|initiator|[identitySet](../resources/identityset.md)|Инициатор события.|
|teamsAppDisplayName|Строка|Отображение имени teamApp.|
|teamsAppId|Строка|Уникальный идентификатор teamsApp.|

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