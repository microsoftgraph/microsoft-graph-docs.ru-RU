---
title: Тип ресурса signInLocation
description: Предоставляет Город, состояние и страны или региона, из которой входа в произошло.
ms.openlocfilehash: a3d4f6ca5ec18e70960f45a3da1bb06d51ee1e65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078908"
---
# <a name="signinlocation-resource-type"></a>Тип ресурса signInLocation
Предоставляет Город, состояние и страны или региона, из которой входа в произошло.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Предоставляет Город, входа в источник. При расчете используется в операции регистрации Широта и долгота сведения.|
|countryOrRegion|String|Предоставляет info код страны (2 код письма) входа в источник.  При расчете используется в операции регистрации Широта и долгота сведения.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Предоставляет широта, долгота и высота входа в источник.|
|state|String|Предоставляет состояние входа в источник. При расчете используется в операции регистрации Широта и долгота сведения.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInLocation"
}-->

```json
{
  "city": "String",
  "countryOrRegion": "String",
  "geoCoordinates": {"@odata.type": "microsoft.graph.geoCoordinates"},
  "state": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->