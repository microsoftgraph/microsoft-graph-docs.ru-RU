---
title: Тип ресурса teamworkBot
description: Бот в экосистеме Microsoft Teams.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3413ee882a7ca387d298b148b37266704558031c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158319"
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

- Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md)
- Чтобы получить боты, установленные в чате, см. пример 2 в [списке приложений в чате.](../api/chat-list-installedapps.md)
- Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в списке [приложений, установленных для пользователя.](../api/userteamwork-list-installedapps.md)



