---
title: Тип ресурса Operation
description: Состояние длительной операции.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: billbliss
ms.openlocfilehash: f57b9f14603fdeae539e872d87b5af2645cedef0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998521"
---
# <a name="operation-resource-type"></a>Тип ресурса Operation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Состояние длительной операции.

## <a name="methods"></a>Методы

Нет

## <a name="properties"></a>Свойства

| Свойство           | Тип            | Описание                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| createdDateTime    | DateTimeOffset  | Время начала операции.                                                |
| id                 | String          | Идентификатор операции. только для чтения. Создается сервером.                                  |
| ластактиондатетиме | DateTimeOffset  | Время последнего действия операции.                                   |
| status             | String          | Возможные значения: `notStarted`, `running`, `completed`, `failed`. Только для чтения. |

## <a name="relationships"></a>Отношения

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>Пример

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


