---
title: тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных в домене.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3d2140d0b0067ec576433b442446472d0a6af80fd4152131ea79d384a8d623c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54218802"
---
# <a name="domainstate-resource-type"></a>тип ресурса domainState

Пространство имен: microsoft.graph

Представляет состояние асинхронных операций, запланированных в домене.

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Timestamp для последнего действия. Значение обновляется, когда запланирована операция, начинается асинхронная задача и когда операция завершается. |
| операция | String | Тип асинхронной операции. Значения могут быть *ForceDelete или* *Проверка* |
| status | String | Текущее состояние операции. <br> *Запланированный* . Операция была запланирована, но не началась. <br> *InProgress* — задача запущена и находится в процессе выполнения. <br> *Failed* - Operation has failed. |

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

