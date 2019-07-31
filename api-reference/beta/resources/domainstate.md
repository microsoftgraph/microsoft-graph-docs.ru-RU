---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 40e3bb3055e0156f00f95598f50a343adc332423
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973099"
---
# <a name="domainstate-resource-type"></a>Тип ресурса Домаинстате

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет состояние асинхронных операций, запланированных в домене.

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
| Ластактиондатетиме | DateTimeOffset | Временная метка времени последнего действия. Значение обновляется при планировании операции асинхронная задача начинается и после завершения операции. |
| восстановление | String | Тип асинхронной операции. Значения могут быть *форцеделете* или *верификацией* |
| status | String | Текущее состояние операции. <br> *Запланированная* операция запланирована, но еще не запущена. <br> *Выполнение* — задача запущена и выполняется. <br> *Failed* — не удалось выполнить операцию. |

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
