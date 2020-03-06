---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: Ресурс GeoCoordinates предоставляет географические координаты и высоту расположения в соответствии с метаданными файла.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c6fce88c0a85b23e799030e9190d7d82e884089d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532930"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="d1530-103">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="d1530-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="d1530-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1530-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d1530-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="d1530-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1530-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1530-107">JSON representation</span></span>

<span data-ttu-id="d1530-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="d1530-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1530-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1530-109">Properties</span></span>

| <span data-ttu-id="d1530-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1530-110">Property</span></span>  | <span data-ttu-id="d1530-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d1530-111">Type</span></span>   | <span data-ttu-id="d1530-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d1530-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="d1530-113">altitude</span><span class="sxs-lookup"><span data-stu-id="d1530-113">altitude</span></span>  | <span data-ttu-id="d1530-114">Double</span><span class="sxs-lookup"><span data-stu-id="d1530-114">Double</span></span> | <span data-ttu-id="d1530-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1530-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="d1530-118">latitude</span><span class="sxs-lookup"><span data-stu-id="d1530-118">latitude</span></span>  | <span data-ttu-id="d1530-119">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="d1530-119">Double</span></span> | <span data-ttu-id="d1530-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1530-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="d1530-123">longitude</span><span class="sxs-lookup"><span data-stu-id="d1530-123">longitude</span></span> | <span data-ttu-id="d1530-124">Double</span><span class="sxs-lookup"><span data-stu-id="d1530-124">Double</span></span> | <span data-ttu-id="d1530-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d1530-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="d1530-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="d1530-128">Remarks</span></span>

<span data-ttu-id="d1530-129">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d1530-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
