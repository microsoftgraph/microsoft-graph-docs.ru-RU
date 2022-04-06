---
title: Тип ресурса associatedTeamInfo
description: Представляет команду, связанную с пользователем.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2e3c8c83d10d5c15595edf9aef8f0b3b50e661e4
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685413"
---
# <a name="associatedteaminfo-resource-type"></a>Тип ресурса associatedTeamInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет команду [,](team.md) связанную с [пользователем](../resources/user.md). В настоящее [время пользователь](../resources/user.md) может быть связан с [командой двумя](../resources/team.md) разными способами:
* Пользователь [может](../resources/user.md) быть непосредственным участником [команды](../resources/team.md).
* Пользователь [может](../resources/user.md) быть членом общего [канала,](../resources/channel.md) размещенного в [команде](../resources/team.md).



Наследуется [от teamInfo](../resources/teaminfo.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление associatedTeamInfo](../api/associatedteaminfo-list.md)|[коллекция associatedTeamInfo](../resources/associatedteaminfo.md)|Получение списка связанных [объектовTeamInfo](../resources/associatedteaminfo.md) и их свойств.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя команды. Наследуется [от teamInfo](../resources/teaminfo.md).|
|tenantId|String|Идентификатор Azure Active Directory клиента. Наследуется [от teamInfo](../resources/teaminfo.md).|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.associatedTeamInfo",
  "baseType": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.associatedTeamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "tenantId": "String"
}
```

## <a name="see-also"></a>См. также
- [Получение команды](../api/team-get.md)