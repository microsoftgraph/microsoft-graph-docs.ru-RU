---
title: тип ресурса printUsageByUser
description: Описывает действия печати для пользователя в течение определенного периода времени (useDate).
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b4809f77e7ceeba79ea5b7e75737fb0750cc4dc
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781298"
---
# <a name="printusagebyuser-resource-type"></a>тип ресурса printUsageByUser

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия печати для пользователя в течение определенного периода времени (useDate).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | Получите список сводок ежедневного использования печати, сгруппив их по пользователю. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | Получите список ежемесячных сводок использования печати, сгруппив их по пользователю. |
| [получение](../api/printusagebyuser-get.md); | [printUsageByUser](printusagebyuser.md) | Чтение свойств и связей объекта printUsageByUser. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|ID этого сводки использования.|
|userPrincipalName|String|UpN пользователя, представленного этими статистическими данными.|
|useDate|Дата|Дата, связанная с этими статистическими данными.|
|completedBlackAndWhiteJobCount|Int64|Количество заданий черной и белой печати, завершенных от имени пользователя в связанную дату.|
|completedColorJobCount|Int64|Количество заданий цветной печати, завершенных от имени пользователя в связанную дату.|
|incompleteJobCount|Int64|Количество заданий печати, которые были в очереди от имени пользователя, но не завершены, в связанную дату.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByUser"
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
  "description": "printUsageByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

