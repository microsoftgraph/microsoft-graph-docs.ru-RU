---
title: тип ресурса operationError
description: Описывает ошибки в teamsAsyncOperation.
ms.localizationpriority: medium
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b30a945dcbd19a6c1be0c276eec0b650b8251ea1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098512"
---
# <a name="operationerror-resource-type"></a>тип ресурса operationError

Пространство имен: microsoft.graph



Описывает ошибки [в teamsAsyncOperation](teamsasyncoperation.md).

## <a name="operationerror-properties"></a>operationError Properties
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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

