---
title: " Тип ресурса secureScoreControlStateUpdate"
description: Этот ресурс содержит журнал обновлен пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).
localization_priority: Normal
ms.openlocfilehash: 4e626f67579e3dc35fe36f5dcc67b1512c5e7bbc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574392"
---
 ##  <a name="securescorecontrolstateupdate-resource-type"></a>Тип ресурса secureScoreControlStateUpdate

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Содержит журнал обновления пользователем состояния элемента управления (элемент управления следующие состояния по умолчанию, игнорируется, сторонних, проверено).

|Свойство         | Тип           |Описание                                                  |
|:----------------|:---------------|:------------------------------------------------------------|
| assignedTo      | string         | Назначение элемента управления для пользователя, который будет выполнять действия     |
| comment         | строка         | Предоставляет дополнительный комментарий об элементе управления                 |
| state           | string         | Состояние элемента управления можно изменить с помощью команды ИСПРАВЛЕНИЯ (Ex: игнорируется, сторонних и т.д.) |
| updatedBy       | string         |Идентификатор пользователя, который обновить состояние клиента                      |
| updatedDateTime | DateTimeOffset |Время, в какой элемент управления обновить состояние                      |
 

## <a name="json-representation"></a>Представление JSON
 Ниже указано представление ресурса в формате JSON.

 <!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
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
