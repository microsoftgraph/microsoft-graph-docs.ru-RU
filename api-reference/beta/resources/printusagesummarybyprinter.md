---
title: Тип ресурса Принтусажесуммарибипринтер
description: Описывает действия печати для принтера в указанный период времени (Усажедате).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070658"
---
# <a name="printusagesummarybyprinter-resource-type"></a>Тип ресурса Принтусажесуммарибипринтер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия печати для принтера в указанный период времени (Усажедате).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [принтусажесуммарибипринтер](printusagesummarybyprinter.md) | Получите список ежедневных сводок использования, сгруппированных по принтерам. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [принтусажесуммарибипринтер](printusagesummarybyprinter.md) | Получение списка ежемесячных сводок использования печати с группировкой по принтерам. |
| [получение](../api/printusagesummarybyprinter-get.md); | [принтусажесуммарибипринтер](printusagesummarybyprinter.md) | Чтение свойств и связей объекта **принтусажесуммарибипринтер** . |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор этой сводки использования.|
|принтерид|String|ИДЕНТИФИКАТОР принтера, представленный данными статистикой.|
|усажедате|Дата|Дата, связанная с этими статистикой.|
|комплетедблаккандвхитежобкаунт|Int64|Количество черно-белых заданий печати, выполненных принтером на связанную дату.|
|комплетедколоржобкаунт|Int64|Число заданий цветной печати, выполненных принтером на связанную дату.|
|инкомплетежобкаунт|Int64|Количество заданий печати, которые были поставлены в очередь для принтера, но не завершены, на соответствующую дату.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
}-->

```json
{
    "id": "String (identifier)",
    "printerId": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

