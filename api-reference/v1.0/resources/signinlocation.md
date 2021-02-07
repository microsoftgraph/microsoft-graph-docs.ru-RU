---
title: Тип ресурса signInLocation
description: Предоставляет город, штат и страну или регион, из которых произошел вход.
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c003fda44e54bbee5957e794d02b90f008f4b8f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137097"
---
# <a name="signinlocation-resource-type"></a>Тип ресурса signInLocation

Пространство имен: microsoft.graph

Предоставляет город, штат и страну или регион, из которых произошел вход.

## <a name="properties"></a>Свойства

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|city|String|Предоставляет город, в котором был произведен вход. Этот метод вычисляется с использованием сведений о широте и долготе из действия при входе.|
|countryOrRegion|String|Предоставляет сведения о коде страны (2 буквы), с которых был произведен вход.  Этот метод вычисляется с использованием сведений о широте и долготе из действия при входе.|
|geoCoordinates|[geoCoordinates](geocoordinates.md)|Предоставляет широту, долготу и высоту, в которой был произведен вход.|
|state|String|Предоставляет состояние, в котором был произведен вход. Это вычисляется с использованием сведений о широте и долготе из действия при входе.|

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

