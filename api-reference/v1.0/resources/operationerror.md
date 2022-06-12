---
title: Тип ресурса operationError
description: Описание ошибок в teamsAsyncOperation.
ms.localizationpriority: medium
author: billbliss
ms.prod: teamwork
doc_type: resourcePageType
ms.openlocfilehash: 0bdc08d7d98b4f926a1cd6a247ccb9b6d41b9d62
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034451"
---
# <a name="operationerror-resource-type"></a>Тип ресурса operationError

Пространство имен: microsoft.graph



Описание ошибок в [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>Свойства operationError
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|string (только для чтения)|Код ошибки операции.|
|сообщение|string (только для чтения)|Сообщение об ошибке операции.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

