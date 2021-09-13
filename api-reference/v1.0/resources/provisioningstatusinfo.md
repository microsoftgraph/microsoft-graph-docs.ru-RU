---
title: provisioningStatusInfo resource type
description: Описывает состояние события сводки по подготовкам.
ms.localizationpriority: medium
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 82b13a700cece9b558ec131f68ea3f79fc0105c2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59052876"
---
# <a name="provisioningstatusinfo-resource-type"></a>provisioningStatusInfo resource type

Пространство имен: microsoft.graph


Описывает состояние события сводки по подготовкам. 

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|status|provisioningResult| Возможные значения: `success`, `warning`, `failure`, `skipped`, `unknownFutureValue`.|
|errorInfo|[provisioningErrorInfo](provisioningErrorInfo.md)| Если состояние не успешно или пропущенные сведения об ошибке содержатся в этом.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningStatusInfo",
  "baseType": null
}-->

```json
{
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningStatusInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


