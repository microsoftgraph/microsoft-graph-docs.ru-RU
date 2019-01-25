---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 45df506820ee242b53630c9d44ed390216bae141
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525075"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="db5bc-102">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="db5bc-102">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db5bc-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="db5bc-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db5bc-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db5bc-105">JSON representation</span></span>

<span data-ttu-id="db5bc-106">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="db5bc-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="db5bc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="db5bc-107">Properties</span></span>

| <span data-ttu-id="db5bc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="db5bc-108">Property</span></span>  | <span data-ttu-id="db5bc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="db5bc-109">Type</span></span>   | <span data-ttu-id="db5bc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="db5bc-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="db5bc-111">altitude</span><span class="sxs-lookup"><span data-stu-id="db5bc-111">altitude</span></span>  | <span data-ttu-id="db5bc-112">Double</span><span class="sxs-lookup"><span data-stu-id="db5bc-112">Double</span></span> | <span data-ttu-id="db5bc-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db5bc-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="db5bc-116">latitude</span><span class="sxs-lookup"><span data-stu-id="db5bc-116">latitude</span></span>  | <span data-ttu-id="db5bc-117">Double</span><span class="sxs-lookup"><span data-stu-id="db5bc-117">Double</span></span> | <span data-ttu-id="db5bc-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db5bc-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="db5bc-121">longitude</span><span class="sxs-lookup"><span data-stu-id="db5bc-121">longitude</span></span> | <span data-ttu-id="db5bc-122">Double</span><span class="sxs-lookup"><span data-stu-id="db5bc-122">Double</span></span> | <span data-ttu-id="db5bc-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="db5bc-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="db5bc-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="db5bc-126">Remarks</span></span>

<span data-ttu-id="db5bc-127">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="db5bc-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location",
  "suppressions": [
    "Error: /api-reference/beta/resources/geocoordinates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
