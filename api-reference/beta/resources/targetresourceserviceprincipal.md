---
title: Тип ресурса targetResourceServicePrincipal
description: Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита. На основе targetResource ресурсов.
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080732"
---
# <a name="targetresourceserviceprincipal-resource-type"></a>Тип ресурса targetResourceServicePrincipal
Указывает ServicePrincipalId для ресурсов, на которые оказывает активности аудита. На основе [targetResource](targetresource.md) ресурсов.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Description|
|:---------------|:--------|:----------|
|appId|String|Указывает уникальный идентификатор приложения. Указатель идентификатор приложения для приложения содержится код.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->