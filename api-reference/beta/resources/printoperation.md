---
title: Тип ресурса Принтоператион
description: Представляет длительную универсальную операцию печати. Базовый класс для типов операций, например Принтеркреатеоператион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 970ac3dd06e5af1478600166ffdd4c84815aa5b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048724"
---
# <a name="printoperation-resource-type"></a>Тип ресурса Принтоператион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет длительную универсальную операцию печати. Базовый класс для типов операций, например [принтеркреатеоператион](printercreateoperation.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение операции](../api/printoperation-get.md) | [printOperation](printoperation.md) | Получение длительной операции в текущем пользователе или клиенте приложения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор операции. Только для чтения.|
|status|[printOperationStatus](printoperationstatus.md)|Состояние операции. Только для чтения.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании операции. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


