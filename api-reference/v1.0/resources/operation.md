---
title: Тип ресурса операции
description: Состояние длительной операции.
ms.localizationpriority: medium
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 58473fcdfdd98a269299aba495cd1bd397423a6d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098526"
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

