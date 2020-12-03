---
title: Тип ресурса Провисионингстеп
description: 'Описывает действия, предпринимаемые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 24685d0d2a25d00b19bcb796ae0df304c8224ebd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523541"
---
# <a name="provisioningstep-resource-type"></a>Тип ресурса Провисионингстеп

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия, предпринимаемые для выполнения действия.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Сводка действий, произошедших на этапе.|
|details|[detailsInfo](detailsinfo.md)|Сведения о том, что произошло на этапе.|
|name|String|Имя этапа.|
|провисионингстептипе|String| Тип этапа. Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|String| Состояние этапа. Возможные значения: `success` ,, `warning`  `failure` , `skipped` , `unknownFutureValue` .|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStep",
  "baseType": null
}-->

```json
{
  "description": "String",
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "name": "String",
  "provisioningStepType": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStep resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


