---
author: JeremyKelley
description: Ресурс "геокоординаты" предоставляет географические координаты и возвышение расположения на основе метаданных, содержащихся в файле.
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 07b0a39155b8c9c4dc02d6cff1e0a93c1a9cd418
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497638"
---
# <a name="geocoordinates-resource-type"></a>Тип ресурса "геокоординаты"

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Предоставляет географические координаты и расширение расположения на основе метаданных, содержащихся в файле.
Если [**driveItem**](driveitem.md) имеет аспект **Location** , отличный от NULL, элемент представляет файл с известным расположением связанной с ним.

> [!NOTE]
> При обновлении широты и долготы фотографии необходимо указать ресурс [Photo](photo.md) (пустой или другой).

## <a name="properties"></a>Свойства

| Свойство  | Тип   | Описание
|:----------|:-------|:--------------------------------------------------------
| altitude  | Double | Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.
| latitude  | Double | Необязательный. Широта элемента (в десятичной системе). Возможность записи в OneDrive персональный.
| longitude | Double | Необязательный. Широта элемента (в десятичном виде). Возможность записи в OneDrive персональный.

## <a name="json-representation"></a>Представление JSON

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
