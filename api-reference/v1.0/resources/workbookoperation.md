---
title: Тип ресурса workbookOperation
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: c674186befbb6a24c41cd8741f554876a17a4394
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158949"
---
# <a name="workbookoperation-resource-type"></a>Тип ресурса workbookOperation

Представляет состояние длительной операции с книгой.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | Получите операцию с `{operation-id}` помощью . |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String| Текущее состояние операции. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|id|String| ИД операции. Только для чтения.|
|error|[workbookOperationError](workbookoperationerror.md)| Ошибка, возвращенная операцией.|
|resourceLocation|String| URI ресурса для результата.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "status": {"@odata.type": "microsoft.graph.workbookOperationStatus"},
  "error": {"@odata.type": "microsoft.graph.workbookOperationError"},
  "resourceLocation": "String",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
