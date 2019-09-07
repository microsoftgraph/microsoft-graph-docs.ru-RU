---
title: Тип ресурса ИнвитепартиЦипантсоператион
description: Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a974bd22ddd9e1ac8c6ab90cdedb9dda9f1a1bb5
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793037"
---
# <a name="inviteparticipantsoperation-resource-type"></a>Тип ресурса ИнвитепартиЦипантсоператион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние длительной операции с приглашением для участников, активируемым при вызове API участника-приглашения.

## <a name="properties"></a>Свойства

| Свойство                       | Тип                        | Описание                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| Контекст                  | String.                      | Контекст клиента.                                                                                                                               |
| createdDateTime                | DateTimeOffset              | Время создания записи.                                                                                                          |
| id                             | Строка                      | Идентификатор операции сервера. Только для чтения. Создается сервером.                                                                                             |
| ластактиондатетиме             | DateTimeOffset              | Время последнего действия операции.                                                                                                     |
| participants | Коллекция [инвитатионпартиЦипантинфо](invitationParticipantInfo.md) | Участники, которые необходимо пригласить. |
| resultInfo                     | [resultInfo](resultinfo.md) | Сведения о результате.  Только для чтения. Создается сервером.                                                                                             |
| status                         | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. Создается сервером.                                                 |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "participants": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inviteParticipantsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
