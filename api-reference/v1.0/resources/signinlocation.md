---
title: тип ресурса signInLocation
description: Предоставляет город, штат и страну/регион, откуда произошла входная программа.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: fb22cf430ec3bffd04150398600beae5af4c41579f00f3cf49196587efb9f44b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124159"
---
# <a name="signinlocation-resource-type"></a>тип ресурса signInLocation

Пространство имен: microsoft.graph

Предоставляет город, штат и страну/регион, откуда произошла входная программа.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Предоставляет город, в котором возникла входная подпись. Это вычисляется с использованием данных о широте и долготе из действия входного знака.|
|countryOrRegion|String|Предоставляет сведения о коде страны (код 2 буквы), откуда возникла входная точка.  Это вычисляется с использованием данных о широте и долготе из действия входного знака.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Обеспечивает широту, долготу и высоту, где возникла входная.|
|state|String|Предоставляет состояние, в котором возникла входная подпись. Это вычисляется с использованием данных о широте и долготе из действия входного знака.|

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

