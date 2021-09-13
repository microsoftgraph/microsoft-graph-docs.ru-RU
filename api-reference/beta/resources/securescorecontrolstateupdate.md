---
title: " secureScoreControlStateUpdate type"
description: Этот ресурс содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 17d35370907ac82d47b28e67b7fb4ba6c0068bb7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063617"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate type
Содержит историю состояния управления, обновляемого пользователем (состояния управления включают Default, Ignored, ThirdParty, Reviewed).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | string | Назначение управления пользователю, который будет принимать действие |
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


