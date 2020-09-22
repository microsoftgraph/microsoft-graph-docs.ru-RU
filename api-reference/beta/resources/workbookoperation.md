---
title: Тип ресурса Воркбукоператион
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 957f94087fa8c11cf3a5cc794bf194e21bbba346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075380"
---
# <a name="workbookoperation-resource-type"></a>Тип ресурса Воркбукоператион

Представляет состояние длительной операции с книгой.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Воркбукоператион](../api/workbookoperation-get.md) | [воркбукоператион](workbookoperation.md) | Получение состояния объекта **воркбукоператион** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Идентификатор операции. только для чтения.|
|status|String| Текущее состояние операции. Возможные значения: `notStarted`, `running`, `succeeded`, `failed`.|
|error|[воркбукоператионеррор](workbookoperationerror.md)| Ошибка, возвращенная операцией.|
|ресаурцелокатион|String| URI ресурса для результата.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookOperation",
  "baseType": "",
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


