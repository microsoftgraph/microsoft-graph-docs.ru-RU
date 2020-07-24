---
title: Тип ресурса Воркбукоператион
description: Представляет состояние длительных операций с книгой.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4fa98cdfdfc013386f7d615c54c832d27c5f826e
ms.sourcegitcommit: 233ac43db0eb5edd46fe944a5515d7dd9abb1298
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2020
ms.locfileid: "45408164"
---
# <a name="workbookoperation-resource-type"></a>Тип ресурса Воркбукоператион

Представляет состояние длительной операции с книгой.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение Воркбукоператион](../api/workbookoperation-get.md) | [воркбукоператион](workbookoperation.md) | Получение операции с помощью `{operation-id}` . |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String| Текущее состояние операции. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|id|Строка| Идентификатор операции. Только для чтения.|
|error|[воркбукоператионеррор](workbookoperationerror.md)| Ошибка, возвращенная операцией.|
|ресаурцелокатион|Строка| URI ресурса для результата.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

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