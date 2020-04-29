---
title: Тип ресурса signInLocation
description: Предоставляет город, область и страну или регион, из которых выполняется вход.
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 58c3dc2b25b85963e6a0f6f88552dbf2a121d5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446858"
---
# <a name="signinlocation-resource-type"></a>Тип ресурса signInLocation

Пространство имен: microsoft.graph

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
