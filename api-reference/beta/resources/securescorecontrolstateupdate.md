---
title: " Тип ресурса secureScoreControlStateUpdate"
description: Этот ресурс содержит журнал состояний элементов управления, обновленных пользователем (состояния элементов управления включают Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 72be4693fa6b851ee587462d96451d78430a24a6
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899513"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса secureScoreControlStateUpdate
Содержит журнал состояний элементов управления, обновленных пользователем (состояния элементов управления включают Default, Ignored, ThirdParty, Reviewed).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | string | Назначьте элемент управления пользователю, который будет выполнять действие |
|comment | string | Предоставляет необязательный комментарий к элементу управления |
|состояние | string | Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.) |
|updatedBy | string |Идентификатор пользователя, который обновил состояние клиента |
|updatedDateTime | DateTimeOffset |Время обновления состояния элемента управления |
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


