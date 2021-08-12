---
title: тип ресурса operationError
description: Описывает ошибки в teamsAsyncOperation.
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 395b10dbfd3617cfe891854897c9d99be64ad4b76bc05776b4eab77d1847a44f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223272"
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

