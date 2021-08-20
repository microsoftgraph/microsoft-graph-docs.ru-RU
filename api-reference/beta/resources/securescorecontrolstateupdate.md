---
title: " secureScoreControlStateUpdate type"
description: Этот ресурс содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9e369cb863981d9998e20c17047899c8d2c02689219bdd0fef2dd56c660076d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176220"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate type
Содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | строка | Назначение управления пользователю, который будет принимать действие |
|comment | string | Предоставляет необязательный комментарий о контроле |
|состояние | string | Состояние управления можно изменить с помощью команды PATCH (Ex: ignored, thirdParty и т.д.) |
|updatedBy | string |ID пользователя, обновившего состояние клиента |
|updatedDateTime | DateTimeOffset |Время обновления состояния управления |
 ## <a name="json-representation"></a>Представление JSON
 Ниже указано представление ресурса в формате JSON.
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


