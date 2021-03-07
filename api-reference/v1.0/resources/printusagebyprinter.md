---
title: тип ресурса printUsageByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8c5a69d01f0b8da05a5f72f5c2c7d9bacf10ff1a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518013"
---
# <a name="printusagebyprinter-resource-type"></a>тип ресурса printUsageByPrinter

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Описывает активность печати для принтера в течение указанного периода времени (useDate).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Получите список ежемесячных сводок использования печати, сгруппив их по принтеру. |
| [получение](../api/printUsageByPrinter-get.md); | [printUsageByPrinter](printUsageByPrinter.md) | Ознакомьтесь с свойствами и отношениями объекта **printUsageByPrinter.** |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID этого сводки использования.|
|printerID|Строка|ID принтера, представленный этими статистическими данными.|
|useDate|Дата|Дата, связанная с этими статистическими данными.|
|completedBlackAndWhiteJobCount|Int64|Количество заданий черной и белой печати, завершенных принтером в связанную дату.|
|completedColorJobCount|Int64|Количество заданий цветного печати, завершенных принтером в связанную дату.|
|incompleteJobCount|Int64|Количество заданий печати, которые были в очереди для принтера, но не завершены, в связанную дату.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "printerId": "String"
}
```

