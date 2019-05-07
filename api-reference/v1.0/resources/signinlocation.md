---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6f81556526c9de1177248b7015bb276e47cb73d9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629238"
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

## <a name="json-representation"></a>Представление в формате JSON

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
