---
title: тип ресурса domainState
description: Представляет состояние асинхронных операций, запланированных в домене.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d69beb993de7bc6e87d5945e321b89e1007c6910
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123729"
---
# <a name="domainstate-resource-type"></a>тип ресурса domainState

Пространство имен: microsoft.graph

Представляет состояние асинхронных операций, запланированных в домене.

## <a name="properties"></a>Свойства

| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
| lastActionDateTime | DateTimeOffset | Timestamp для последнего действия. Значение обновляется, когда запланирована операция, начинается асинхронная задача и когда операция завершается. |
| операция | Строка | Тип асинхронной операции. Значения могут быть *ForceDelete или* *Проверка* |
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

