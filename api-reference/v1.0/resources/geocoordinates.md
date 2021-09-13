---
author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
ms.localizationpriority: medium
description: Ресурс GeoCoordinates предоставляет географические координаты и высоту расположения в соответствии с метаданными файла.
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: c5039586f44ae5b3dc73c59004a68afccee63a30
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094326"
---
# <a name="geocoordinates-resource-type"></a>Тип ресурса GeoCoordinates

Пространство имен: microsoft.graph

Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.

## <a name="json-representation"></a>Представление JSON

Ниже показано представление JSON ресурса.

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

## <a name="properties"></a>Свойства

| Свойство  | Тип   | Описание
|:----------|:-------|:--------------------------------------------------------
| altitude  | Double | Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.
| latitude  | Double | Необязательный. Широта элемента (в десятичной системе). Только для чтения.
| longitude | Double | Необязательный. Широта элемента (в десятичном виде). Только для чтения.

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->

