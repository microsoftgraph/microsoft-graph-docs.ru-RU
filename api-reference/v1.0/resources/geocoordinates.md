---
author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: Ресурс GeoCoordinates предоставляет географические координаты и высоту расположения в соответствии с метаданными файла.
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: b2c6fec5e27e3b8fe902b330b226fc498b09b138
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240012"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="a1ce6-103">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a1ce6-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="a1ce6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1ce6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1ce6-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a1ce6-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1ce6-107">JSON representation</span></span>

<span data-ttu-id="a1ce6-108">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="a1ce6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1ce6-109">Properties</span></span>

| <span data-ttu-id="a1ce6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1ce6-110">Property</span></span>  | <span data-ttu-id="a1ce6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a1ce6-111">Type</span></span>   | <span data-ttu-id="a1ce6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ce6-112">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="a1ce6-113">altitude</span><span class="sxs-lookup"><span data-stu-id="a1ce6-113">altitude</span></span>  | <span data-ttu-id="a1ce6-114">Double</span><span class="sxs-lookup"><span data-stu-id="a1ce6-114">Double</span></span> | <span data-ttu-id="a1ce6-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="a1ce6-118">latitude</span><span class="sxs-lookup"><span data-stu-id="a1ce6-118">latitude</span></span>  | <span data-ttu-id="a1ce6-119">Double</span><span class="sxs-lookup"><span data-stu-id="a1ce6-119">Double</span></span> | <span data-ttu-id="a1ce6-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="a1ce6-123">longitude</span><span class="sxs-lookup"><span data-stu-id="a1ce6-123">longitude</span></span> | <span data-ttu-id="a1ce6-124">Double</span><span class="sxs-lookup"><span data-stu-id="a1ce6-124">Double</span></span> | <span data-ttu-id="a1ce6-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="a1ce6-128">Заметки</span><span class="sxs-lookup"><span data-stu-id="a1ce6-128">Remarks</span></span>

<span data-ttu-id="a1ce6-129">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a1ce6-129">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->

