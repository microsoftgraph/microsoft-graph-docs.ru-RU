---
title: Тип ресурса teamInfo
description: Представляет команду с базовой информацией.
author: devjha-ms
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0e2d683428dae15a0b51989906dbb9ecac16b945
ms.sourcegitcommit: c21fefa5c3c62df14147e7918cb43327f7d72e69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/06/2022
ms.locfileid: "64685343"
---
# <a name="teaminfo-resource-type"></a>Тип ресурса teamInfo

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет команду [с базовой](team.md) информацией.

Базовый тип [связанных объектовTeamInfo](associatedteaminfo.md) и [sharedWithChannelTeamInfo](sharedwithchannelteaminfo.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Имя команды.|
|tenantId|String|Идентификатор Azure Active Directory клиента.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamInfo",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamInfo",
  "displayName": "String",
  "id": "String (identifier)",
  "tenantId": "String"
}
```
