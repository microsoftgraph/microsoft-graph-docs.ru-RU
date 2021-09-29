---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0c4bc7721566bd8210830e51dbe820b1b44813e1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996369"
---
# <a name="conditionalaccessdevices-resource-type"></a>тип ресурса conditionalAccessDevices

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройства в области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeDevices | Коллекция String | Состояния в области политики. `All` является единственным допустимым значением. Невозможно установить, если *установлено устройствоFIlter.* |
| excludeDevices | Коллекция String | Государства, исключенные из сферы действия политики. Возможные значения: `Compliant` , `DomainJoined` . Невозможно установить, если **установлено устройствоFIlter.** |
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Фильтр, определяющее правило динамического устройства и синтаксиса для включаемых и исключаемых устройств. Фильтр может использовать свойства устройств (например, атрибуты расширения), чтобы включить или исключить их. Невозможно установить, **если задают includeDevices** или **excludeDevices.** |
| includeDeviceStates (deprecated)| Коллекция String | Состояния в области политики. `All` является единственным допустимым значением. |
| excludeDeviceStates (deprecated)| Коллекция String | Государства, исключенные из сферы действия политики. Возможные значения: `Compliant` , `DomainJoined` . |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices",
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ],
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


