---
title: тип ресурса workbookOperation
description: Представляет состояние длительных операций с книгами.
ms.localizationpriority: medium
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: e27d38aa1c04ca3be43955d15131b927f89fa5cc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59119746"
---
# <a name="workbookoperation-resource-type"></a>тип ресурса workbookOperation

Представляет состояние длительной операции книг.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | Извлечение состояния **объекта workbookOperation.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| ID операции. Только для чтения.|
|status|String| Текущее состояние операции. Возможные значения: `notStarted`, `running`, `succeeded`, `failed`.|
|error|[workbookOperationError](workbookoperationerror.md)| Ошибка, возвращаемая операцией.|
|resourceLocation|String| Ресурс URI для результата.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

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
  "resourceLocation": "String"
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


