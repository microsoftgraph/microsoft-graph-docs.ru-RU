---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
ms.localizationpriority: medium
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 419a9b92626fb3c3693f5974119d677ef50d5b26
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561754"
---
# <a name="conditionalaccessdevices-resource-type"></a>тип ресурса conditionalAccessDevices

Пространство имен: microsoft.graph

Представляет устройства в области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Фильтр, определяющее правило динамического устройства и синтаксиса для включаемых и исключаемых устройств. Фильтр может использовать свойства устройств (например, атрибуты расширения), чтобы включить или исключить их. |

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


