---
title: тип ресурса printUsageSummaryByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753613"
---
# <a name="printusagesummarybyprinter-resource-type"></a>тип ресурса printUsageSummaryByPrinter

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает активность печати для принтера в течение указанного периода времени (useDate).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | Получите список ежемесячных сводок использования печати, сгруппив их по принтеру. |
| [получение](../api/printusagesummarybyprinter-get.md); | [printUsageSummaryByPrinter](printusagesummarybyprinter.md) | Ознакомьтесь с свойствами и отношениями объекта **printUsageSummaryByPrinter.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|ID этого сводки использования.|
|printerID|String|ID принтера, представленный этими статистическими данными.|
|useDate|Дата|Дата, связанная с этими статистическими данными.|
|completedBlackAndWhiteJobCount|Int64|Количество заданий черной и белой печати, завершенных принтером в связанную дату.|
|completedColorJobCount|Int64|Количество заданий цветного печати, завершенных принтером в связанную дату.|
|incompleteJobCount|Int64|Количество заданий печати, которые были в очереди для принтера, но не завершены, в связанную дату.|

## <a name="json-representation"></a>Представление в формате JSON

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

