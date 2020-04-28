---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92616569a87a6ccf91c17ea7c845b8185bd33e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965231"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса Секурескореконтролстатеупдате
Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | string | Назначение элемента управления пользователю, который будет выполнять действие |
|comment | string | Предоставляет необязательный комментарий об элементе управления |
|состояние | string | Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.) |
|упдатедби | string |Идентификатор пользователя, который обновил состояние клиента |
|упдатеддатетиме | DateTimeOffset |Время обновления состояния элемента управления |
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
