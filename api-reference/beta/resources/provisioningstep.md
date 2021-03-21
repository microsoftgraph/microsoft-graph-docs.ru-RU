---
title: тип ресурса provisioningStep
description: 'Описывает действия, предпринятые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6baf1656cb470cfc8dc01908f5a398ac5d421eb1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960343"
---
# <a name="provisioningstep-resource-type"></a>тип ресурса provisioningStep

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Описывает действия, предпринятые для выполнения действия.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|Строка|Сводка о том, что произошло во время шага.|
|подробности|[detailsInfo](detailsinfo.md)|Сведения о том, что произошло во время шага.|
|name|String|Имя шага.|
|provisioningStepType|provisioningStepType| Тип шага. Возможные значения: `import`, `scoping`, `matching`, `processing`, `referenceResolution`, `export`, `unknownFutureValue`.|
|status|provisioningResult| Состояние шага. Возможные значения: `success` `warning` , , ,  `failure` `skipped` `unknownFutureValue` .|

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


