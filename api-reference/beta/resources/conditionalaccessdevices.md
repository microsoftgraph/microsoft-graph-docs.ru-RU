---
title: тип ресурса conditionalAccessDevices
description: Представляет устройства в области политики.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cbb542420228a4a383dea4e165323fbb6e8abb17
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082358"
---
# <a name="conditionalaccessdevices-resource-type"></a>тип ресурса conditionalAccessDevices

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет устройства в области политики.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
| includeDevices | Коллекция объектов string | Состояния в области политики. `All` является единственным допустимым значением. Невозможно установить, если *установлено устройствоFIlter.* |
| excludeDevices | Коллекция объектов string | Государства, исключенные из сферы действия политики. Возможные значения: `Compliant` , `DomainJoined` . Невозможно установить, если **установлено устройствоFIlter.** |
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Фильтр, определяющий правило динамического устройства и синтаксиса, чтобы включить или исключить устройства. Фильтр может использовать свойства устройств (например, атрибуты расширения), чтобы включить или исключить их. Невозможно установить, **если задают includeDevices** или **excludeDevices.** |
| includeDeviceStates (deprecated)| Коллекция объектов string | Состояния в области политики. `All` является единственным допустимым значением. |
| excludeDeviceStates (deprecated)| Коллекция объектов string | Государства, исключенные из сферы действия политики. Возможные значения: `Compliant` , `DomainJoined` . |

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


