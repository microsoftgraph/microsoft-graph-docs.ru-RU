---
title: тип ресурса signInLocation
description: Предоставляет город, штат и страну/регион, откуда произошла входная программа.
ms.localizationpriority: medium
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 826daa833829b8ca9da9f4844827b308c8843044
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139599"
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

