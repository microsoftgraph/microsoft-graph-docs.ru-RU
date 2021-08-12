---
title: Тип ресурса операции
description: Состояние длительной операции.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b1aabcf259d2d185d24b07e25b79d97e928ee245fd4f11acd848bc4f4a1ed646
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180588"
---
# <a name="operation-resource-type"></a>Тип ресурса операции

Пространство имен: microsoft.graph

Состояние длительной операции.

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|createdDateTime| DateTimeOffset |Время начала операции.|
|lastActionDateTime| DateTimeOffset |Время последнего действия операции.|
|status|operationStatus|Текущий статус операции: `notStarted` , `running` , `completed``failed` |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

