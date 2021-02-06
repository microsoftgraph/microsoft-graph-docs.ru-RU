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
# <a name="geocoordinates-resource-type"></a><span data-ttu-id="dff91-103">Тип ресурса geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="dff91-103">geoCoordinates resource type</span></span>

<span data-ttu-id="dff91-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dff91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dff91-105">Предоставляет географические координаты и повышение прав расположения на основе метаданных, содержащихся в файле.</span><span class="sxs-lookup"><span data-stu-id="dff91-105">Provides geographic coordinates and elevation of a location based on metadata contained within the file.</span></span>
<span data-ttu-id="dff91-106">Если [**у элемента driveItem**](driveitem.md) есть  аспект расположения, не нулевой, элемент представляет файл с известным расположением, в который он вошел.</span><span class="sxs-lookup"><span data-stu-id="dff91-106">If a [**driveItem**](driveitem.md) has a non-null **location** facet, the item represents a file with a known location assocaited with it.</span></span>

> [!NOTE]
> <span data-ttu-id="dff91-107">При обновлении широты и долготы фотографии необходимо предоставлять ресурс [фотографии](photo.md) (пустой или иным образом).</span><span class="sxs-lookup"><span data-stu-id="dff91-107">When updating the latitude and longitude of a photo, a [photo](photo.md) resource (empty or otherwise) must be provided.</span></span>

## <a name="properties"></a><span data-ttu-id="dff91-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="dff91-108">Properties</span></span>

| <span data-ttu-id="dff91-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dff91-109">Property</span></span>  | <span data-ttu-id="dff91-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dff91-110">Type</span></span>   | <span data-ttu-id="dff91-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dff91-111">Description</span></span>
|:----------|:-------|:--------------------------------------------------------
| <span data-ttu-id="dff91-112">altitude</span><span class="sxs-lookup"><span data-stu-id="dff91-112">altitude</span></span>  | <span data-ttu-id="dff91-113">Double</span><span class="sxs-lookup"><span data-stu-id="dff91-113">Double</span></span> | <span data-ttu-id="dff91-p102">Необязательный. Высота элемента над уровнем моря (в футах). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="dff91-p102">Optional. The altitude (height), in feet,  above sea level for the item. Read-only.</span></span>
| <span data-ttu-id="dff91-117">latitude</span><span class="sxs-lookup"><span data-stu-id="dff91-117">latitude</span></span>  | <span data-ttu-id="dff91-118">Double</span><span class="sxs-lookup"><span data-stu-id="dff91-118">Double</span></span> | <span data-ttu-id="dff91-119">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="dff91-119">Optional.</span></span> <span data-ttu-id="dff91-120">Широта элемента (в десятичной системе).</span><span class="sxs-lookup"><span data-stu-id="dff91-120">The latitude, in decimal, for the item.</span></span> <span data-ttu-id="dff91-121">Можно перезаписать в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="dff91-121">Writable on OneDrive Personal.</span></span>
| <span data-ttu-id="dff91-122">longitude</span><span class="sxs-lookup"><span data-stu-id="dff91-122">longitude</span></span> | <span data-ttu-id="dff91-123">Double</span><span class="sxs-lookup"><span data-stu-id="dff91-123">Double</span></span> | <span data-ttu-id="dff91-124">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="dff91-124">Optional.</span></span> <span data-ttu-id="dff91-125">Широта элемента (в десятичном виде).</span><span class="sxs-lookup"><span data-stu-id="dff91-125">The longitude, in decimal, for the item.</span></span> <span data-ttu-id="dff91-126">Можно перезаписать в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="dff91-126">Writable on OneDrive Personal.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dff91-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dff91-127">JSON representation</span></span>

<span data-ttu-id="dff91-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dff91-128">Here is a JSON representation of the resource</span></span>

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


