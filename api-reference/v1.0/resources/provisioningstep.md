---
title: тип ресурса provisioningStep
description: 'Описывает действия, предпринятые для выполнения действия. '
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 9841a70c0f3a00e3d4c163b9f814ae50c2a8221e6a33a1468d29832d5798c495
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231518"
---
# <a name="provisioningstep-resource-type"></a>тип ресурса provisioningStep

Пространство имен: microsoft.graph

Описывает действия, предпринятые для выполнения действия.

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|description|String|Сводка о том, что произошло во время шага.|
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


