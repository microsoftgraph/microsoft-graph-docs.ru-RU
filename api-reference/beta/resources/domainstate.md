---
title: Тип ресурса Домаинстате
description: Представляет состояние асинхронных операций, запланированных в домене.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39ded8e4ff3458ebaceea09b3003d0bd14be36cf
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543184"
---
# <a name="domainstate-resource-type"></a>Тип ресурса Домаинстате

Представляет состояние асинхронных операций, запланированных в домене.

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
| Ластактиондатетиме | DateTimeOffset | Временная метка времени последнего действия. Значение обновляется при планировании операции асинхронная задача начинается и после завершения операции. |
| восстановление | String | Тип асинхронной операции. Значения могут быть *форцеделете* или *верификацией* |
| status | String | Текущее состояние операции. <br> *Запланированная* операция запланирована, но еще не запущена. <br> *Выполнение* — задача запущена и выполняется. <br> *Failed* — не удалось выполнить операцию. |

## <a name="json-representation"></a>Представление в формате JSON
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
