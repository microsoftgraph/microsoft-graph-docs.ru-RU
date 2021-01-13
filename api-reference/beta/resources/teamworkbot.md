---
title: Тип ресурса teamworkBot
description: Бот в экосистеме Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8c21e7ab3b88c2659bf055e39b931cbc6e9d2f39
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844678"
---
# <a name="teamworkbot-resource-type"></a>Тип ресурса teamworkBot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет бота в экосистеме Microsoft Teams.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить бота](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|Чтение свойств и связей объекта [teamworkBot.](../resources/teamworkbot.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД бота, связанного с определенным [teamsAppDefinition.](../resources/teamsappdefinition.md) Обычно это значение является GUID.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamworkBot",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkBot",
  "id": "String (identifier)"
}
```

## <a name="see-also"></a>См. также

- Чтобы получить ботов, установленных в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md)
- Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](../api/chat-list-installedapps.md)
- Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](../api/userteamwork-list-installedapps.md)



