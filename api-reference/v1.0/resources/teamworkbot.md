---
title: тип ресурса teamworkBot
description: Бот в Microsoft Teams экосистеме.
author: AkJo
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0f2c558bc5453f3cf8a880f1935b3f891ba097f7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59055838"
---
# <a name="teamworkbot-resource-type"></a>тип ресурса teamworkBot

Пространство имен: microsoft.graph

Представляет бот в экосистеме Microsoft Teams.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить бот](../api/teamworkbot-get.md)|[teamworkBot](../resources/teamworkbot.md)|Ознакомьтесь с свойствами и отношениями объекта [teamworkBot.](../resources/teamworkbot.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID бота, связанного с [определенными группамиAppDefinition.](../resources/teamsappdefinition.md) Это значение обычно является GUID.|

## <a name="relationships"></a>Отношения
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

- Чтобы получить боты, установленные в команде, см. пример 2 в [списке приложений в команде.](../api/team-list-installedapps.md) <!-- - To get bots installed in a chat, see example 2 in [List apps in chat](../api/chat-list-installedapps.md). -->
- Чтобы получить боты, установленные в личной области пользователя, см. пример 2 в [приложениях List, установленных для пользователя.](../api/userteamwork-list-installedapps.md)



