---
title: " Тип ресурса Секурескореконтролстатеупдате"
description: Этот ресурс содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).
localization_priority: Normal
ms.openlocfilehash: 24febeb4bfb055e89e59cdb4f79c8b60c6c40347
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343362"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса Секурескореконтролстатеупдате
Содержит историю состояний элементов управления, обновленных пользователем (состояния элементов управления включают значение по умолчанию, игнорируется, ThirdParty, проверено).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | string | Назначение элемента управления пользователю, который будет выполнять действие |
|comment | строка | Предоставляет необязательный комментарий об элементе управления |
|состояние | string | Состояние элемента управления можно изменить с помощью команды PATCH (например, игнорируется, thirdParty и т. д.) |
|Упдатедби | string |Идентификатор пользователя, который обновил состояние клиента |
|Упдатеддатетиме | DateTimeOffset |Время обновления состояния элемента управления |
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
