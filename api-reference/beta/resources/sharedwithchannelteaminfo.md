---
title: Тип ресурса sharedWithChannelTeamInfo
description: Представляет команду, которой предоставлен общий доступ к каналу.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 15f6e3138d24bf93a2546be404c21e6bcf4b6daa
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061002"
---
# <a name="sharedwithchannelteaminfo-resource-type"></a>Тип ресурса sharedWithChannelTeamInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения для [команды](team.md), которой предоставлен общий доступ к каналу. [Команда](team.md) может совместно использовать несколько каналов.


Наследуется от [teamInfo](../resources/teaminfo.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получить sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-list.md)|Коллекция [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Получение списка объектов [объектовWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md) и их свойств.|
|[Получить sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-get.md)|[sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md)|Чтение свойств и связей объекта [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md).|
|[Удаление sharedWithChannelTeamInfo](../api/sharedwithchannelteaminfo-delete.md)|Нет|Удаление объекта [sharedWithChannelTeamInfo](../resources/sharedwithchannelteaminfo.md).|
|[Список allowedMembers](../api/sharedwithchannelteaminfo-list-allowedmembers.md)|Коллекция [conversationMember](../resources/conversationmember.md)|Получение списка участников команды, у которых есть доступ к общему каналу.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя команды. Наследуется от [teamInfo](../resources/teaminfo.md).|
|isHostTeam|Логическое|Указывает, является ли [команда](team.md) местом размещения [канала](channel.md).|
|tenantId|String|Идентификатор клиента Azure Active Directory. Наследуется от [teamInfo](../resources/teaminfo.md).|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|allowedMembers|Коллекция [conversationMember](../resources/conversationmember.md)|Коллекция участников команды, у которых есть доступ к общему каналу.|


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

