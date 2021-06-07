---
title: тип ресурса printUsageByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 2826e73ef68d9ee2162c6a2de0bbaba351fd87bd
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781307"
---
# <a name="printusagebyprinter-resource-type"></a>тип ресурса printUsageByPrinter

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает активность печати для принтера в течение указанного периода времени (useDate).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Получите список ежемесячных сводок использования печати, сгруппив их по принтеру. |
| [получение](../api/printUsageByPrinter-get.md); | [printUsageByPrinter](printUsageByPrinter.md) | Ознакомьтесь с свойствами и отношениями объекта **printUsageByPrinter.** |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|ID этого сводки использования.|
|printerID|String|ID принтера, представленный этими статистическими данными.|
|useDate|Дата|Дата, связанная с этими статистическими данными.|
|completedBlackAndWhiteJobCount|Int64|Количество заданий черной и белой печати, завершенных принтером в связанную дату.|
|completedColorJobCount|Int64|Количество заданий цветного печати, завершенных принтером в связанную дату.|
|incompleteJobCount|Int64|Количество заданий печати, которые были в очереди для принтера, но не завершены, в связанную дату.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByPrinter"
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
  "description": "printUsageByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

