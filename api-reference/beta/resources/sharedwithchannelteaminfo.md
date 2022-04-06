---
title: Тип ресурса sharedWithChannelTeamInfo
description: Представляет команду, доступную каналу.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e26bc3db8359ccb560e2922dcb6c8b8328fc2b74
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685336"
---
# <a name="sharedwithchannelteaminfo-resource-type"></a>Тип ресурса sharedWithChannelTeamInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет команду [, доступную](team.md) каналу. Команда [может](team.md) совместно использоваться несколькими каналами.


Наследуется [от teamInfo](../resources/teaminfo.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-list.md)|[Коллекция sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Получение списка общих [объектовWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) и их свойств.|
|[Получение sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Чтение свойств и связей общего [объектаWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) .|
|[Удаление sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-delete.md)|Никаких других изменений не происходит|Удаление объекта [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) .|
|[Перечисление allowedMembers](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|Коллекция [conversationMember](../resources/conversationmember.md)|Получение списка участников команды, имеющих доступ к общему каналу.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя команды. Наследуется [от teamInfo](../resources/teaminfo.md).|
|isHostTeam|Логический|Указывает, является [ли команда](team.md) узлом [канала](channel.md).|
|tenantId|String|Идентификатор Azure Active Directory клиента. Наследуется [от teamInfo](../resources/teaminfo.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|allowedMembers|Коллекция [conversationMember](../resources/conversationmember.md)|Коллекция членов команды, имеющих доступ к общему каналу.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedWithChannelTeamInfo",
  "baseType": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedWithChannelTeamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "isHostTeam": "Boolean",
  "tenantId": "String"
}
```

