---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 19da0630abf4b27899af9e5c6be12254d91e9499
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657695"
---
# <a name="domainstate-resource-type"></a>Тип ресурса Домаинстате

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
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
