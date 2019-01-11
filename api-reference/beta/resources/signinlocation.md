---
title: Тип ресурса signInLocation
description: Предоставляет Город, состояние и страны или региона, из которой входа в произошло.
localization_priority: Normal
ms.openlocfilehash: 49d6dfb07c635ac3754b3e873d75911a43593a73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839139"
---
# <a name="signinlocation-resource-type"></a>Тип ресурса signInLocation
Предоставляет Город, состояние и страны или региона, из которой входа в произошло.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Предоставляет Город, входа в источник. При расчете используется в операции регистрации Широта и долгота сведения.|
|countryOrRegion|Строка|Предоставляет info код страны (2 код письма) входа в источник.  При расчете используется в операции регистрации Широта и долгота сведения.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Предоставляет широта, долгота и высота входа в источник.|
|state|Строка|Предоставляет состояние входа в источник. При расчете используется в операции регистрации Широта и долгота сведения.|

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
