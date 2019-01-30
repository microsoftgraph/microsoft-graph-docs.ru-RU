---
title: " Тип ресурса secureScoreControlStateUpdate"
description: Этот ресурс содержит журнал обновлен пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641731"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса secureScoreControlStateUpdate
Содержит журнал обновления пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).

|Свойство |Тип |Описание |
|:--|:--|:--|
|assignedTo | строка | Назначение элемента управления для пользователя, который будет выполнять действия |
|comment | строка | Предоставляет дополнительный комментарий об элементе управления |
|state | строка | Состояние элемента управления можно изменить с помощью команды ИСПРАВЛЕНИЯ (Ex: игнорируется, сторонних и т.д.) |
|updatedBy | строка |Идентификатор пользователя, который обновить состояние клиента |
|updatedDateTime | DateTimeOffset? |Время, в какой элемент управления обновить состояние |
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
