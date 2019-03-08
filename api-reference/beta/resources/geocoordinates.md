---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: GeoCoordinates
localization_priority: Normal
ms.openlocfilehash: 221037578e055e5bb57987058a190bc3026b3e0c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482359"
---
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="2ab97-102">Тип ресурса GeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="2ab97-102">GeoCoordinates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ab97-p101">Ресурс **GeoCoordinates** предоставляет географические координаты и высоту расположения в соответствии с метаданными файла. Если у ресурса [**DriveItem**](driveitem.md) есть ненулевой аспект **location**, то этот ресурс представляет файл, с которым связано известное расположение.</span><span class="sxs-lookup"><span data-stu-id="2ab97-p101">The **GeoCoordinates** resource provides geographic coordinates and elevation of a location based on metadata contained within the file. If a [**DriveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ab97-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ab97-105">JSON representation</span></span>

<span data-ttu-id="2ab97-106">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ab97-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="2ab97-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ab97-107">Properties</span></span>

| <span data-ttu-id="2ab97-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ab97-108">Property</span></span>  | <span data-ttu-id="2ab97-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ab97-109">Type</span></span>   | <span data-ttu-id="2ab97-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ab97-110">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="2ab97-111">altitude</span><span class="sxs-lookup"><span data-stu-id="2ab97-111">altitude</span></span>  | <span data-ttu-id="2ab97-112">Double</span><span class="sxs-lookup"><span data-stu-id="2ab97-112">Double</span></span> | <span data-ttu-id="2ab97-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ab97-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="2ab97-116">latitude</span><span class="sxs-lookup"><span data-stu-id="2ab97-116">latitude</span></span>  | <span data-ttu-id="2ab97-117">Double</span><span class="sxs-lookup"><span data-stu-id="2ab97-117">Double</span></span> | <span data-ttu-id="2ab97-p103">Необязательный. Широта элемента (в десятичной системе). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ab97-p103">Optional. The latitude, in decimal, for the item. Read-only.</span></span>
| <span data-ttu-id="2ab97-121">longitude</span><span class="sxs-lookup"><span data-stu-id="2ab97-121">longitude</span></span> | <span data-ttu-id="2ab97-122">Double</span><span class="sxs-lookup"><span data-stu-id="2ab97-122">Double</span></span> | <span data-ttu-id="2ab97-p104">Необязательный. Широта элемента (в десятичном виде). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2ab97-p104">Optional. The longitude, in decimal, for the item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="2ab97-126">Заметки</span><span class="sxs-lookup"><span data-stu-id="2ab97-126">Remarks</span></span>

<span data-ttu-id="2ab97-127">Дополнительные сведения об аспектах ресурса DriveItem см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="2ab97-127">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
