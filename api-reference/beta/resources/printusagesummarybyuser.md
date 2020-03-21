---
title: Тип ресурса Принтусажесуммарибюсер
description: Описывает действия печати для пользователя в указанный период времени (Усажедате).
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 30769d9bd7ee76494b1582a3d7afc8a7f75bb07a
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895984"
---
# <a name="printusagesummarybyuser-resource-type"></a>Тип ресурса Принтусажесуммарибюсер

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия печати для пользователя в указанный период времени (Усажедате).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [принтусажесуммарибюсер](printusagesummarybyuser.md) | Получение списка сводных сведений об использовании печати, сгруппированных по пользователям. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [принтусажесуммарибюсер](printusagesummarybyuser.md) | Получение списка ежемесячных сводок использования печати, сгруппированных по пользователям. |
| [получение](../api/printusagesummarybyuser-get.md); | [принтусажесуммарибюсер](printusagesummarybyuser.md) | Чтение свойств и связей объекта Принтусажесуммарибюсер. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|Строка|Идентификатор этой сводки использования.|
|userPrincipalName|String|Имя участника-пользователя, представленное этой статистикой.|
|усажедате|Дата|Дата, связанная с этими статистикой.|
|комплетедблаккандвхитежобкаунт|Int64|Количество черно-белых заданий печати, выполненных от имени пользователя на соответствующую дату.|
|комплетедколоржобкаунт|Int64|Число заданий цветной печати, выполненных от имени пользователя на соответствующую дату.|
|инкомплетежобкаунт|Int64|Количество заданий печати, которые были поставлены в очередь от имени пользователя, но не завершены, на соответствующую дату.|

## <a name="json-representation"></a>Представление JSON

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