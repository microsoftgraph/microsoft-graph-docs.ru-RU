---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf0cdec3a2c5feae1b178fc92d02e433d87737a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965028"
---
# <a name="signinlocation-resource-type"></a>Тип ресурса signInLocation
Предоставляет город, область и страну или регион, из которых выполняется вход.



## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Предоставляет город, в котором поступил вход. Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.|
|countryOrRegion|String|Предоставляет сведения о коде страны (код из 2 букв), где поступил вход.  Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Предоставляет широту, долготу и высоту, на которой поступил вход.|
|state|String|Предоставляет состояние, в котором поступил вход. Рассчитывается с использованием информации о широте и долготе из действия, выполняемого при входе.|

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
