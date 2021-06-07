---
title: тип ресурса printUsageSummaryByUser
description: Описывает действия печати для пользователя в течение определенного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bba9f57799a36bef4a90b7c514a5be4b4846565e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753610"
---
# <a name="printusagesummarybyuser-resource-type"></a>тип ресурса printUsageSummaryByUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия печати для пользователя в течение определенного периода времени (useDate).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | Получите список сводок ежедневного использования печати, сгруппив их по пользователю. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [printUsageSummaryByUser](printusagesummarybyuser.md) | Получите список ежемесячных сводок использования печати, сгруппив их по пользователю. |
| [получение](../api/printusagesummarybyuser-get.md); | [printUsageSummaryByUser](printusagesummarybyuser.md) | Чтение свойств и связей объекта printUsageSummaryByUser. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|ID этого сводки использования.|
|userPrincipalName|String|UpN пользователя, представленного этими статистическими данными.|
|useDate|Дата|Дата, связанная с этими статистическими данными.|
|completedBlackAndWhiteJobCount|Int64|Количество заданий черной и белой печати, завершенных от имени пользователя в связанную дату.|
|completedColorJobCount|Int64|Количество заданий цветной печати, завершенных от имени пользователя в связанную дату.|
|incompleteJobCount|Int64|Количество заданий печати, которые были в очереди от имени пользователя, но не завершены, в связанную дату.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
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
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

