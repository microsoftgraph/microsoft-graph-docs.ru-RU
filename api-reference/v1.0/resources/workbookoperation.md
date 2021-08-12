---
title: тип ресурса workbookOperation
description: Представляет состояние длительных операций с книгами.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fe2cb3a1b899fb1aa9cef1fdc863a7d4432ead8877fed92bb0a53e40b62dd455
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54221147"
---
# <a name="workbookoperation-resource-type"></a>тип ресурса workbookOperation

Представляет состояние длительной операции книг.


## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get workbookOperation](../api/workbookoperation-get.md) | [workbookOperation](workbookoperation.md) | Получите операцию `{operation-id}` с помощью . |


## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|String| Текущее состояние операции. Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.|
|id|String| ID операции. Только для чтения.|
|error|[workbookOperationError](workbookoperationerror.md)| Ошибка, возвращаемая операцией.|
|resourceLocation|String| Ресурс URI для результата.|

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
