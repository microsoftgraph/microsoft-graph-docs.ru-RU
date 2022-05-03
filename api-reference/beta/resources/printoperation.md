---
title: Тип ресурса printOperation
description: Представляет долго выполняющуюся операцию универсальной печати. Базовый класс для типов операций, таких как printerCreateOperation.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 5e3d53d9fbdc5fbb4dd1bda2aa477581df5c838e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176662"
---
# <a name="printoperation-resource-type"></a>Тип ресурса printOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет долго выполняющуюся операцию универсальной печати. Базовый класс для типов операций, таких [как printerCreateOperation](printercreateoperation.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Операция Get](../api/printoperation-get.md) | [printOperation](printoperation.md) | Получение длительной операции в клиенте текущего пользователя или приложения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор операции. Только для чтения.|
|status|[printOperationStatus](printoperationstatus.md)|Состояние операции. Только для чтения.|
|createdDateTime|DateTimeOffset|DateTimeOffset при создании операции. Только для чтения.|

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


