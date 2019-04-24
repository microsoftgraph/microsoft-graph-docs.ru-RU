---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 221037578e055e5bb57987058a190bc3026b3e0c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506339"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="be05e-102">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="be05e-102">GeoCoordinates resource type</span></span>

<span data-ttu-id="be05e-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="be05e-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be05e-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be05e-105">JSON representation</span></span>

<span data-ttu-id="be05e-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="be05e-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="be05e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="be05e-107">Properties</span></span>

| <span data-ttu-id="be05e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="be05e-108">Property</span></span>  | <span data-ttu-id="be05e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="be05e-109">Type</span></span>   | <span data-ttu-id="be05e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be05e-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="be05e-111">altitude</span><span class="sxs-lookup"><span data-stu-id="be05e-111">altitude</span></span>  | <span data-ttu-id="be05e-112">Double</span><span class="sxs-lookup"><span data-stu-id="be05e-112">Double</span></span> | <span data-ttu-id="be05e-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be05e-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="be05e-116">latitude</span><span class="sxs-lookup"><span data-stu-id="be05e-116">latitude</span></span>  | <span data-ttu-id="be05e-117">Double</span><span class="sxs-lookup"><span data-stu-id="be05e-117">Double</span></span> | <span data-ttu-id="be05e-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be05e-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="be05e-121">longitude</span><span class="sxs-lookup"><span data-stu-id="be05e-121">longitude</span></span> | <span data-ttu-id="be05e-122">Double</span><span class="sxs-lookup"><span data-stu-id="be05e-122">Double</span></span> | <span data-ttu-id="be05e-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="be05e-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="be05e-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="be05e-126">Remarks</span></span>

<span data-ttu-id="be05e-127">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="be05e-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
