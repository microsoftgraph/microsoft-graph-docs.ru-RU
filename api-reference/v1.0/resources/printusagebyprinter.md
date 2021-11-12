---
title: тип ресурса printUsageByPrinter
description: Описывает активность печати для принтера в течение указанного периода времени (useDate).
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 31d298ddbb46d615fc805aa92700cd6839d268a0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2021
ms.locfileid: "60944251"
---
# <a name="printusagebyprinter-resource-type"></a>тип ресурса printUsageByPrinter

Пространство имен: microsoft.graph

Описывает активность печати для принтера в течение указанного периода времени (useDate).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Получите список сводок об использовании ежедневной печати, сгруппив их по принтеру. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagebyprinter.md) | [printUsageByPrinter](printUsageByPrinter.md) | Получите список ежемесячных сводок использования печати, сгруппив их по принтеру. |
| [Получение](../api/printUsageByPrinter-get.md); | [printUsageByPrinter](printUsageByPrinter.md) | Ознакомьтесь с свойствами и отношениями объекта **printUsageByPrinter.** |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
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

