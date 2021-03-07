---
title: тип ресурса printUsageByUser
description: Описывает действия печати для пользователя в течение определенного периода времени (useDate).
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c478a4f9827de96d4db0da5d8533628bd8468d98
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518012"
---
# <a name="printusagebyuser-resource-type"></a>тип ресурса printUsageByUser

Пространство имен: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Описывает действия печати для пользователя в течение определенного периода времени (useDate).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Список (ежедневно)](../api/reportroot-list-dailyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | Получите список сводок ежедневного использования печати, сгруппив их по пользователю. |
| [Список (ежемесячно)](../api/reportroot-list-monthlyprintusagebyuser.md) | [printUsageByUser](printusagebyuser.md) | Получите список ежемесячных сводок использования печати, сгруппив их по пользователю. |
| [получение](../api/printusagebyuser-get.md); | [printUsageByUser](printusagebyuser.md) | Чтение свойств и связей объекта printUsageByUser. |

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|ID этого сводки использования.|
|userPrincipalName|String|UpN пользователя, представленного этими статистическими данными.|
|useDate|Дата|Дата, связанная с этими статистическими данными.|
|completedBlackAndWhiteJobCount|Int64|Количество заданий черной и белой печати, завершенных от имени пользователя в связанную дату.|
|completedColorJobCount|Int64|Количество заданий цветной печати, завершенных от имени пользователя в связанную дату.|
|incompleteJobCount|Int64|Количество заданий печати, которые были в очереди от имени пользователя, но не завершены, в связанную дату.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByUser",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "userPrincipalName": "String"
}
```

