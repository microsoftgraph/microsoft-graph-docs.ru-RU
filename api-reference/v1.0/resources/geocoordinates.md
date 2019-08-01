---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
description: Ресурс GeoCoordinates предоставляет географические координаты и высоту расположения в соответствии с метаданными файла.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 64b81bc2946658ffc8617662879bc6cb20e25047
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029311"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="ab010-103">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="ab010-103">GeoCoordinates resource type</span></span>

<span data-ttu-id="ab010-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="ab010-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab010-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ab010-106">JSON representation</span></span>

<span data-ttu-id="ab010-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="ab010-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="ab010-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ab010-108">Properties</span></span>

| <span data-ttu-id="ab010-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ab010-109">Property</span></span>  | <span data-ttu-id="ab010-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ab010-110">Type</span></span>   | <span data-ttu-id="ab010-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ab010-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="ab010-112">altitude</span><span class="sxs-lookup"><span data-stu-id="ab010-112">altitude</span></span>  | <span data-ttu-id="ab010-113">Double</span><span class="sxs-lookup"><span data-stu-id="ab010-113">Double</span></span> | <span data-ttu-id="ab010-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab010-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="ab010-117">latitude</span><span class="sxs-lookup"><span data-stu-id="ab010-117">latitude</span></span>  | <span data-ttu-id="ab010-118">Двойное</span><span class="sxs-lookup"><span data-stu-id="ab010-118">Double</span></span> | <span data-ttu-id="ab010-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab010-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="ab010-122">longitude</span><span class="sxs-lookup"><span data-stu-id="ab010-122">longitude</span></span> | <span data-ttu-id="ab010-123">Double</span><span class="sxs-lookup"><span data-stu-id="ab010-123">Double</span></span> | <span data-ttu-id="ab010-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ab010-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="ab010-127">Заметки</span><span class="sxs-lookup"><span data-stu-id="ab010-127">Remarks</span></span>

<span data-ttu-id="ab010-128">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="ab010-128">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
