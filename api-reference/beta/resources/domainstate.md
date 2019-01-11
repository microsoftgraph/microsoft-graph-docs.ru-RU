---
title: Тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных для домена.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 3701e80c5104c80eae0cdfb4b1b9f549177a2cbf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830221"
---
# <a name="domainstate-resource-type"></a>Тип ресурса domainState

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет состояние асинхронных операций, запланированных для домена.

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Метка времени возникновения последнего действия. Это значение обновляется при планировании операции, запуске асинхронной задачи и завершении операции. |
| операция | String | Тип асинхронной операции. Возможные значения: *ForceDelete* или *Verification*. |
| status | String | Текущее состояние операции. <br> *Scheduled* — операция запланирована, но еще не запущена. <br> *InProgress* — операция запущена и в настоящее время выполняется. <br> *Failed* — не удалось выполнить операцию. |

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
