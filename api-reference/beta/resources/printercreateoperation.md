---
title: Тип ресурса Принтеркреатеоператион
description: Представляет длительную операцию регистрации принтеров. Производный от Принтоператион.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 3ae18e201f5b768de9cc1456de186fdd6b9336b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048857"
---
# <a name="printercreateoperation-resource-type"></a>Тип ресурса Принтеркреатеоператион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет длительную операцию регистрации принтеров. Производный от [принтоператион](printoperation.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение операции](../api/printoperation-get.md) | [printOperation](printoperation.md) | Получение длительной операции в текущем пользователе или клиенте приложения. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор операции. Только для чтения.|
|status|[printOperationStatus](printoperationstatus.md)|Состояние операции регистрации. Содержит ход выполнения операции, а также сведения о ее успешном выполнении. Только для чтения.|
|createdDateTime|DateTimeOffset|Значение DateTimeOffset при создании операции. Только для чтения.|
|certificate|String|Подписанный сертификат, созданный в процессе регистрации. Только для чтения.|
|Printer|[Printer](printer.md)|Созданная сущность принтера. Только для чтения.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
    "id": "String (identifier)",
    "status": {"@odata.type": "microsoft.graph.printOperationStatus"},
    "createdDateTime": "2020-06-15T19:54:14.853Z",
    "certificate": "",
    "printer": {"@odata.type": "microsoft.graph.printer"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printerCreateOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

