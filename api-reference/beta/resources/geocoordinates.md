---
author: JeremyKelley
description: Ресурс geoCoordinates предоставляет географические координаты и повышение прав расположения на основе метаданных, содержащихся в файле.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: e3b0ac4f616afe648b5c30dc9d15978036a7ab80
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129424"
---
# <a name="geocoordinates-resource-type"></a>Тип ресурса geoCoordinates

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет географические координаты и повышение прав расположения на основе метаданных, содержащихся в файле.
Если [**у элемента driveItem**](driveitem.md) есть  аспект расположения, не нулевой, элемент представляет файл с известным расположением, в который он вошел.

> [!NOTE]
> При обновлении широты и долготы фотографии необходимо предоставлять ресурс [фотографии](photo.md) (пустой или иным образом).

## <a name="properties"></a>Свойства

| Свойство  | Тип   | Описание
|:----------|:-------|:--------------------------------------------------------
| altitude  | Double | Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.
| latitude  | Double | Необязательный. Широта элемента (в десятичной системе). Можно перезаписать в OneDrive персональный.
| longitude | Double | Необязательный. Широта элемента (в десятичном виде). Можно перезаписать в OneDrive персональный.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": []
}
-->


