---
title: Тип ресурса Коммсоператион
description: Состояние определенных длительных операций.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a10b652179a8a3d369c07d34cb2681c4986b3abf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012900"
---
# <a name="commsoperation-resource-type"></a>Тип ресурса Коммсоператион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Состояние определенных длительных операций.

## <a name="methods"></a>Методы
Нет

## <a name="properties"></a>Свойства

| Свойство           | Тип                        | Описание                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| Контекст      | String                      | Контекст клиента.                                                             |
| createdDateTime    | DateTimeOffset              | Время начала операции.                                                |
| id                 | Строка                      | Идентификатор операции. Только для чтения. Создается сервером.                                  |
| Ластактиондатетиме | DateTimeOffset              | Время последнего действия операции.                                   |
| resultInfo         | [resultInfo](resultinfo.md) | Сведения о результате. Только для чтения. Создается сервером.                            |
| status             | String                      | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. |

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
