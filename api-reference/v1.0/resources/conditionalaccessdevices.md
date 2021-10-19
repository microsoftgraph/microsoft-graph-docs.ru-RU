---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
ms.localizationpriority: medium
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8da01cf7a0fbaf1af41550d7b334099a9d34b3e5
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60488855"
---
# <a name="conditionalaccessdevices-resource-type"></a>тип ресурса conditionalAccessDevices

Пространство имен: microsoft.graph

Представляет устройства в области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Фильтр определяет правило динамического устройства-синтаксиса для включаемого или исключаемого устройства. Фильтр может использовать свойства устройств (например, атрибуты расширения), чтобы включить или исключить их. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "deviceFilter": {"@odata.type": "microsoft.graph.conditionalAccessFilter"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDevices resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


