---
title: " Тип ресурса secureScoreControlStateUpdate"
description: Этот ресурс содержит журнал обновлен пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380968"
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
