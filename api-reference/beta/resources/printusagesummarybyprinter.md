---
title: Тип ресурса Принтусажесуммарибипринтер
description: Описывает действия печати для принтера в указанный период времени (Усажедате).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 86d7b4eb107ac6e2732e32bf55a65a7125edb529
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42896053"
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