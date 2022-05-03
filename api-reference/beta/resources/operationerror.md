---
title: Тип ресурса operationError
description: Описание ошибок в teamsAsyncOperation.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: teamwork
author: billbliss
ms.openlocfilehash: 3634e55dca6328b40a9d21577183e8a5616c53f8
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176509"
---
# <a name="operationerror-resource-type"></a>Тип ресурса operationError

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описание ошибок в [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>Свойства operationError
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|code|string (только для чтения)|Код ошибки операции.|
|message|string (только для чтения)|Сообщение об ошибке операции.|

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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


