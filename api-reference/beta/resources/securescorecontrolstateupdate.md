---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549141"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса Секурескореконтролстатеупдате
Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | string | Назначение элемента управления пользователю, который будет выполнять действие |
|comment | строка | Предоставляет необязательный комментарий об элементе управления |
|состояние | string | Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.) |
|Упдатедби | string |Идентификатор пользователя, который обновил состояние клиента |
|Упдатеддатетиме | DateTimeOffset? |Время обновления состояния элемента управления |
 ## <a name="json-representation"></a>Представление в формате JSON
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
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
